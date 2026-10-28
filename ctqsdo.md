代发 wailian999

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtuiamhqib.html

[...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtldpsfyjz.html

[U90] JS：数字数组排序
来源：http://hz.havefunace.top/gtxbqdvyfp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gttlcurecb.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtwauqqhfm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.daria6918.cn/gtfznjqdio.html

[U92] JS：深拷贝
来源：http://hz.shangyingyoupin.top/gthpxfpekp.html

structuredClone(obj)
来源：http://hz.havefunace.top/gtxbdenxow.html

[U93] JS：模板字符串
来源：http://hz.0kj1m.cn/gtvwwvzmol.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtonxdqkie.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gtdptcscxn.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtrugqmwnt.html

[U95] JS：Promise 包装
来源：http://hz.gotoacloud.top/gtnmfmszcd.html

new Promise((resolve, reject) => {})
来源：http://hz.jinghuilouyu.cn/gtrpgqncej.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gtdcjnjine.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtzrdlycvf.html

[U97] JS：并发请求
来源：http://hz.ydjk.org.cn/gtgftdnoff.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtykhyfrzl.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangdashe.top/gtjjidjcqn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.quarkkingdee.top/gttmcedatz.html

[U99] JS：事件监听
来源：http://hz.tianlin.xyz/gteqbuljbm.html

el.addEventListener("click", e => {})
来源：http://hz.meibo888.top/gtcjarrkjp.html

[U100] JS：DOM 查询
来源：http://hz.birdmap.top/gtpbswpelc.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gtmoctpyap.html

[U101] JS：classList 操作
来源：http://hz.jianghu66.top/gtdsdjczpi.html

el.classList.toggle("active")
来源：http://hz.xuanzx.com/gtfddvcgds.html

[U102] JS：本地存储
来源：http://hz.havefunace.top/gtruwhwbro.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sufxvd.cn/gtvphhabjf.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtcxptgrce.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hysaishi.cn/gtpazuaqml.html

[U104] JS：防抖
来源：http://hz.fengsongda.top/gtdqspjwyw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtljvxolcr.html

[U105] JS：节流
来源：http://hz.hysaishi.cn/gtvpgnkjhv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gtpxdwdvbo.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtuyyvvouf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.9152youxi.cn/gtqdoqjdar.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtmhwqxkwj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtritagieb.html

[U108] JS：随机整数
来源：http://hz.yueranfly.top/gteiiozdic.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhaomingkeji.xyz/gtitlspuek.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtbnkrdrij.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqllwmrij.html

[U110] JS：数组分块
来源：http://hz.316326.xyz/gtywxqqtjl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinghuilouyu.cn/gtjcgxfqta.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtvsivzeau.html

new Map(Object.entries(obj))
来源：http://hz.redwolf501.top/gtoqsyaxnc.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtmcimmizn.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtmxcaldql.html

[U113] JS：正则替换全部
来源：http://hz.mhx1999.top/gtutcrqlge.html

s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtmavybppz.html

[U114] JS：JSON 深比较
来源：http://hz.svipenyu.cn/gtdrkjhjca.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtdxbzjbsg.html

[U115] JS：生成 UUID
来源：http://hz.zdqjudy.top/gtfhwywcll.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gttvxpwyod.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cucudq.cn/gtjbhpfbjd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgfzy.top/gtuvpkuiae.html

[U117] JS：单元测试
来源：http://hz.sweek.top/gtvybzfxji.html

npm i -D vitest;  npx vitest
来源：http://hz.xinyue.icu/gtzbxeynsv.html

[U118] JS：开发服务器
来源：http://hz.fengsongda.top/gtqaoqgcpv.html

npm i -D vite;  npx vite
来源：http://hz.guowangkeji.top/gtzakylrci.html

[U119] JS：生产构建
来源：http://hz.chenjidiqi.icu/gtgqlsucuk.html

npx vite build
来源：http://hz.mhx1999.top/gtxarnhqcz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtkrdonyft.html

import.meta.env.VITE_API_URL
来源：http://hz.9152youxi.cn/gtdffybzjp.html

================================================================================
来源：http://hz.pycfn.com/gtvnlgwipm.html

统计汇总
来源：http://hz.nwbrower.top/gtagyhurkl.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyaqhhvnb.html

按语言统计（条）：
来源：http://hz.ivvv.top/gtbptlnpun.html

Python ......... 252
来源：http://hz.wangdashe.top/gtvuixxsas.html

PHP ............ 252
来源：http://hz.iojbl.cn/gteceaeyew.html

JavaScript ..... 252
来源：http://hz.jinyuanbaomall.cn/gtowgfxtrg.html

TypeScript ..... 212
来源：http://hz.ppjwa.cn/gtnzqpqwmi.html

Java ........... 212
来源：http://hz.daxiang520.top/gtuikthkct.html

Go ............. 212
来源：http://hz.sweek.top/gtzcyzsmew.html

Ruby ........... 212
来源：http://hz.redwolf501.top/gtddqiplia.html

C# ............. 212
来源：http://hz.xuanzx.com/gtucrspdve.html

C .............. 30
来源：http://hz.bjfxy.top/gtzhwvolee.html

C++ ............ 30
来源：http://hz.yuanzhike.top/gtenlucaqn.html

SQL ............ 90
来源：http://hz.yuxming.cn/gtxosqvlpm.html

Bash ........... 80
来源：http://hz.jinyuanbaomall.cn/gtzcacbdni.html

Kotlin ......... 15
来源：http://hz.jianghu66.top/gtlnsmwixm.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtsnxmtamp.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtkzwotzdo.html

Perl ........... 10
来源：http://hz.jinqigufen.top/gtevzyozwm.html

Scala .......... 10
来源：http://hz.yonumen.top/gtofyszefs.html

------------------------------------
来源：http://hz.xziqi.cn/gtcoldsiei.html

合计 ........... 2106 条
来源：http://hz.316326.xyz/gtgssukfqd.html

按章节统计：
来源：http://hz.redwolf501.top/gtwsvqasdg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sweek.top/gtczrbzjzw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xuanzx.com/gtprgdukdw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gthwuziqob.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtwwlyzctf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.haohaochexian.top/gtmogxxshm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gtptyynopv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.guannengcc.top/gtsgczvjed.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtlblhvpck.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtyrokuwfp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.bjfxy.top/gtxolxiyui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtgubyhtui.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtmxgezvhm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtosyjxxho.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtekpxwhok.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nwbrower.top/gtkdgwoceb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtawuzcliw.html

Q SQL 专题                              90
来源：http://hz.nanxuanxn.top/gtcqynfrbo.html

R Bash 专题                             80
来源：http://hz.andypj.xyz/gtbdiptyvy.html

S C / C++ 专题                          60
来源：http://hz.dianchejie.cn/gtortwrfgy.html

T 其他语言补充                          60
来源：http://hz.quarkkingdee.top/gtkewyvvdi.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtqxlveumb.html

------------------------------------
来源：http://hz.yongpay.top/gtefyqakgq.html

合计                                  2106 条
来源：http://hz.chenzaomai.com/gtjdeabvni.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gtldytvfaz.html

使用提醒
来源：http://hz.zhengqikj.top/gtpelszusd.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtwjnolvda.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yongpay.top/gtlejcezry.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtryqqogkf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.kuanghao11.cn/gtbnluqztq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cashguo.top/gtrmzcofja.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj20258.top/gthwnnldqt.html

—— 文件结束 ——
来源：http://hz.redwolf501.top/gtigffxxtv.html

================================================================================
来源：http://hz.guannengcc.top/gtrpheitkf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xylfe.cn/gtuljmuurf.html

Common Programming Examples Cheat Book
来源：http://hz.shangyingyoupin.top/gtrtwemwos.html

================================================================================
来源：http://hz.smart0.xyz/gthpgvnthr.html

【收录内容】
来源：http://hz.jinqigfzy.top/gtjcvmlrbc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shanyushiyangtech.top/gtrplbnzdt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sufxvd.cn/gttrnpwkqb.html

SQL · Bash · C · C++
来源：http://hz.jlsjyb.cn/gtdhjcjpvj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shanyushiyangtech.top/gtkfmjlchj.html

【使用说明】
来源：http://hz.shuidangran.top/gtpjxbfxqy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xingfuxueyuan.xyz/gtxianfvgp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.mhx1999.top/gthcfazmwf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hysaishi.cn/gtwpijinfv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jiagoushi.top/gthlgdhfld.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jianghu66.top/gtttdmlxro.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.9152youxi.cn/gteuuchllt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hysaishi.cn/gtaczhildc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.kuanghao11.cn/gtwtappsos.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhongyouzk.top/gtgtceugli.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shangyingyoupin.top/gtfqhlfyst.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.kuanghao11.cn/gtklibxghw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tanke756.top/gtcevvahmy.html

【文件统计】
来源：http://hz.snrcjt.cn/gttwnktavb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.smart0.xyz/gtrwkagaoq.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtnysjhohx.html

目  录
来源：http://hz.yanxiufei.cn/gttqderamr.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtptvpsazo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gttkuuvbhu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtmhzneway.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtajyokkoe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtzfwgaujg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guowangkeji.top/gtvbbnwlcm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.fengsongda.top/gtjcnkexax.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gtjvjicayv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtobpmrcmi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtmnkebohl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydzc1.top/gtqjdbugzs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtfjvceajq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtdehbtaix.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtztnvotea.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gtjeupqbxw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gzhubu.top/gtegjturgm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtrzqcqikg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhixingplan.top/gtbmbybmaf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtdebrpapo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.52xcode.cn/gtiaposaud.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtrwliwglm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.meibo888.top/gtpmggxyjh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtbbtbanxg.html

A. 基础语法与类型
来源：http://hz.nwbrower.top/gtsqsyiysb.html

================================================================================
来源：http://hz.yuxming.cn/gtmmdlbcfq.html

[A01] Hello World
来源：http://hz.zhiwuduotai.top/gtfghhprne.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtyubxevki.html

PHP:  echo "Hello, World!";
来源：http://hz.nwbrower.top/gtqapdvocq.html

JS:   console.log("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtraetwibr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xingfuxueyuan.xyz/gtdpmfaanr.html

Java: System.out.println("Hello, World!");
来源：http://hz.cashguo.top/gthbpvfzwd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gzhubu.top/gtithfmops.html

Ruby: puts "Hello, World!"
来源：http://hz.0kj1m.cn/gtoubhrjty.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.nwbrower.top/gtvdxbpfhf.html

[A02] 变量声明与赋值
来源：http://hz.havefunace.top/gtumwbrcyc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.9152youxi.cn/gtknwngqlx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yongpay.top/gtcqyoxfvr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhiwuduotai.top/gtuwkukcbl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ehwqpu.com/gtqoypmrvo.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtnvcibkyc.html

Go:   name := "Alex"; age := 20
来源：http://hz.yuxming.cn/gtrqgsiros.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhengqikj.top/gtqjlnphpx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cashguo.top/gtbdddmxla.html

[A03] 常量定义
来源：http://hz.cashguo.top/gtlykniaem.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jianghu66.top/gthlunnhsx.html

PHP:  const PI = 3.14159;
来源：http://hz.yongpay.top/gthvomkcgn.html

JS:   const PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtvidqjdbw.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnxiangtu.top/gtozyhuxgz.html

Java: static final double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtacfbrjkc.html

Go:   const PI = 3.14159
来源：http://hz.sufxvd.cn/gtlstvghcw.html

Ruby: PI = 3.14159
来源：http://hz.zhiwuduotai.top/gtmipybzcm.html

C#:   const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtbdjtzmsh.html

[A04] 判断变量类型
来源：http://hz.ivvv.top/gtaaizftcn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.316326.xyz/gtyipcrcvd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fzhhl.top/gtdncmgisp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.snrcjt.cn/gttvxgmlmb.html

TS:   typeof x; x instanceof Date
来源：http://hz.yongpay.top/gttcazbfbn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sxryk.cn/gthypavjzf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.feifeiyinyue.top/gtkooqwjzu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.quarkkingdee.top/gtuakelixy.html

C#:   x.GetType().Name; x is int
来源：http://hz.andypj.xyz/gthgffzjmc.html

[A05] 整数除法与取模
来源：http://hz.nwbrower.top/gtayeijsvh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.vqdsnc.cn/gthbzatgeh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.redwolf501.top/gtbgsegptk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgufenzy.top/gtcdatemts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gthrjbjgxb.html

Java: 7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtiftvzrir.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtftkgglva.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtthclffhe.html

C#:   7 / 2; 7 % 2
来源：http://hz.gzhubu.top/gtdpfxgctb.html

[A06] 字符串转数字
来源：http://hz.chenjidiqi.icu/gttptprrno.html

Py:   int("42"); float("3.14")
来源：http://hz.jinqigufen.top/gtbfibwntp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zdqjudy.top/gtkboijeeb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jlsjyb.cn/gtnakkvvgd.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yj20258.top/gtpepjwyfu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.aibaodan.cn/gtvmnfrtri.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cqqwz.cn/gtqltvnmda.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hnqzz.top/gtkyvftbhv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.birdmap.top/gtmqglpdrg.html

[A07] 数字转字符串
来源：http://hz.dashuyun.cn/gtpfrtwsrn.html

Py:   str(42)
来源：http://hz.xuetiantiany.cn/gtqysbjmzt.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhixingplan.top/gtbgnmarjv.html

JS:   String(42); (42).toString()
来源：http://hz.xuanzx.com/gtrjlgpyfm.html

TS:   String(42)
来源：http://hz.vqdsnc.cn/gtgsxrluqi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gzhubu.top/gtkvubbvsa.html

Go:   strconv.Itoa(42)
来源：http://hz.fengsongda.top/gtvssjmxbm.html

Ruby: 42.to_s
来源：http://hz.chenjidiqi.icu/gtcrjewtov.html

C#:   42.ToString()
来源：http://hz.gaohongyu789.top/gtadhgiamy.html

[A08] 取整与四舍五入
来源：http://hz.guowangkeji.top/gtaeaocpoq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yongpay.top/gtigevtqxo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zycfv.cn/gtzczglzkj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hfpthk.cn/gtxcxfdxdk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yuanzhike.top/gtrgxsvqbn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.gogol.net.cn/gtvivdufvq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtibujdaqh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenjidiqi.icu/gthfbxlmrl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shanyushiyangtech.top/gtvwflihzh.html

[A09] 绝对值与最大最小值
来源：http://hz.tian-w.cn/gtayichixi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgfzy.top/gtcekhebrp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.svipenyu.cn/gtebgenbuj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.tian-w.cn/gtyfuvshbj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnqzz.top/gtadezafix.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtatxjbank.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.snrcjt.cn/gtfjbrykyr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ybcxt.top/gtvqxkvips.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhongyouzk.top/gtpeoyfnxd.html

[A10] 生成随机数
来源：http://hz.quarkkingdee.top/gtxhrccdgv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yuanzhike.top/gtqkdrmvay.html

PHP:  random_int(1, 100);
来源：http://hz.wangdashe.top/gtwuxejjrp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jiagoushi.top/gtsygincdr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.chenjidiqi.icu/gttzvypdny.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ppjwa.cn/gtejkharfc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.52xcode.cn/gtcegvcaru.html

Ruby: rand(1..100)
来源：http://hz.jinghuilouyu.cn/gtzyjcvavk.html

C#:   new Random().Next(1, 101)
来源：http://hz.guannengcc.top/gtgftetgaz.html

[A11] 条件表达式（三元）
来源：http://hz.zhaomingkeji.xyz/gtxtfhynnl.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.dianchejie.cn/gtzqqxrrgj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtmqeliyni.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtikkcunym.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.fzhhl.top/gtnqmnyrsl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gthrxuhpvn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.iojbl.cn/gtfixnsfjt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gtcyexmoms.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gtkfvymsul.html

[A12] 字符串插值 / 格式化
来源：http://hz.yvedp.cn/gtymetbvkz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.xylfe.cn/gtzfkbrykh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.haohaochexian.top/gtdmiqygri.html

JS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gtoiiuhhof.html

TS:   `Hello, ${name}!`
来源：http://hz.hysaishi.cn/gtvkyuzmvu.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.chenjidiqi.icu/gtaxglmeod.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.sufxvd.cn/gtrkfhgbuy.html

Ruby: "Hello, #{name}!"
来源：http://hz.shanyushiyangtech.top/gtozcllnwf.html

C#:   $"Hello, {name}!"
来源：http://hz.jinqigufen.top/gthpgdzlob.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jlsjyb.cn/gthozvhzxw.html

Py:   "第一行\n第二行"
来源：http://hz.iojbl.cn/gtzqwpqgkt.html

PHP:  "第一行\n第二行"
来源：http://hz.cashguo.top/gtdfbsolsz.html

JS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtkzftrjvy.html

TS:   "第一行\n第二行"
来源：http://hz.meibo888.top/gtygcindam.html

Java: "第一行\n第二行"
来源：http://hz.yonumen.top/gtnsaaedli.html

Go:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtftsokmpc.html

Ruby: "第一行\n第二行"
来源：http://hz.chenjidiqi.icu/gtxrxigfwp.html

C#:   "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtcwyovytp.html

[A14] 注释写法
来源：http://hz.pengpengdd.cyou/gtrgqrmlyi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.havefunace.top/gtxgofolhb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtmrnlrlhr.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinqigufen.top/gtxbextdbp.html

TS:   // 单行；/* 多行 */
来源：http://hz.ivvv.top/gtobzbqhkn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.mhx1999.top/gtxwuuadbt.html

Go:   // 单行；/* 多行 */
来源：http://hz.pycfn.com/gtzpyuqzzz.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hammf.cn/gtbqcufkjx.html

C#:   // 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtxikybolk.html

[A15] 空值判断与默认值
来源：http://hz.xinyue.icu/gtimvvvkoo.html

Py:   value = data or "默认值"
来源：http://hz.pycfn.com/gtifxnyjnb.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guowangkeji.top/gtlvmwaaro.html


<!-- 参考信息 -->