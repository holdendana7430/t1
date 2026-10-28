代发 wailian999

[U93] JS：模板字符串
来源：http://hz.quarkkingdee.top/gtyrygfcao.html

`共 ${n} 条`
来源：http://hz.zdqjudy.top/gtnuueznad.html

[U94] JS：箭头函数
来源：http://hz.tianlin.xyz/gtxnjnacpk.html

const double = x => x * 2;
来源：http://hz.kuanghao11.cn/gtkpmwtonx.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gtfwkbdppw.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtpktzihha.html

[U96] JS：async/await 与异常
来源：http://hz.hnxiangtu.top/gtzdgkhmbm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtwqckpucd.html

[U97] JS：并发请求
来源：http://hz.xylfe.cn/gtukmyfvkw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtserocybu.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhaomingkeji.xyz/gttwzbubex.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cucudq.cn/gttbdvwdaq.html

[U99] JS：事件监听
来源：http://hz.yuxming.cn/gthyyquqrg.html

el.addEventListener("click", e => {})
来源：http://hz.ppjwa.cn/gtehrpbrnp.html

[U100] JS：DOM 查询
来源：http://hz.xuetiantiany.cn/gtyefyojjw.html

document.querySelector(".item")
来源：http://hz.gotoacloud.top/gtfkcovelg.html

[U101] JS：classList 操作
来源：http://hz.yj202588.top/gtnppcreaz.html

el.classList.toggle("active")
来源：http://hz.yj20258.top/gtnsylfvol.html

[U102] JS：本地存储
来源：http://hz.chenzaomai.com/gtvkrekvuk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinyuanbaomall.cn/gtzehgxipm.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtjlhyxadq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ivvv.top/gtiwpxmxfc.html

[U104] JS：防抖
来源：http://hz.cdnleiting.top/gtyiciglbw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtgoenuweo.html

[U105] JS：节流
来源：http://hz.zhaomingkeji.xyz/gtdbdcluge.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shzxlz.cn/gtvkklvwyj.html

[U106] JS：日期格式化
来源：http://hz.jinghuilouyu.cn/gtceonptfp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtrdoxbsws.html

[U107] JS：数字千分位
来源：http://hz.ydzc1.top/gtpkfhbncb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zycfv.cn/gtaawsfban.html

[U108] JS：随机整数
来源：http://hz.ydzc1.top/gtglpvejpn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.svipenyu.cn/gtsohficbe.html

[U109] JS：数组分组
来源：http://hz.hnqzz.top/gtiwxnzaoa.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtdjxmigji.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gtzhkeznbn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yanxiufei.cn/gtsruxwiik.html

[U111] JS：对象转 Map
来源：http://hz.chenjidiqi.icu/gtdslqwafr.html

new Map(Object.entries(obj))
来源：http://hz.quarkkingdee.top/gtwacjcvex.html

[U112] JS：字符串补位
来源：http://hz.daxiang520.top/gtrhbpfxri.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtdikssomc.html

[U113] JS：正则替换全部
来源：http://hz.gzhubu.top/gtgzqlxmve.html

s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtpzkjadqc.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtkjqbxqmo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtfwkpuaif.html

[U115] JS：生成 UUID
来源：http://hz.xylfe.cn/gtjwyfomup.html

crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtudgkjsrk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cheryme.top/gtrkelsbat.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gthckpyghf.html

[U117] JS：单元测试
来源：http://hz.cqqwz.cn/gtdwgvyzxf.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgfzy.top/gttfngzshg.html

[U118] JS：开发服务器
来源：http://hz.dianchejie.cn/gttmyiqxge.html

npm i -D vite;  npx vite
来源：http://hz.jinyuanbaomall.cn/gtlgxtwaem.html

[U119] JS：生产构建
来源：http://hz.chenzaomai.com/gtujniuhju.html

npx vite build
来源：http://hz.cdnleiting.top/gtyrlivxed.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinqigufen.top/gtxvtnulnv.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258.top/gtzsstkmdv.html

================================================================================
来源：http://hz.sweek.top/gtzgjyehrq.html

统计汇总
来源：http://hz.xylfe.cn/gtuaqczakl.html

================================================================================
来源：http://hz.gotoacloud.top/gtpjzjxmde.html

按语言统计（条）：
来源：http://hz.yangfankeji.com/gtqaqfhmrr.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtkiwzvxdy.html

PHP ............ 252
来源：http://hz.xinyue.icu/gtdwyiwwbi.html

JavaScript ..... 252
来源：http://hz.hfpthk.cn/gtllniztds.html

TypeScript ..... 212
来源：http://hz.bjfxy.top/gtlvfqwasz.html

Java ........... 212
来源：http://hz.sxryk.cn/gtgeyjjtdp.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtiexidbii.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtzvuksozh.html

C# ............. 212
来源：http://hz.ydjk.org.cn/gtffzosxbp.html

C .............. 30
来源：http://hz.redwolf501.top/gtzewuhlor.html

C++ ............ 30
来源：http://hz.ywan-chungtsiang.top/gttutbqyhx.html

SQL ............ 90
来源：http://hz.ywan-chungtsiang.top/gtzstvckdr.html

Bash ........... 80
来源：http://hz.yj20258.top/gtemodxrfv.html

Kotlin ......... 15
来源：http://hz.xuanzx.com/gtypibrpim.html

Swift .......... 15
来源：http://hz.nanxinkj.top/gtqoducskh.html

Lua ............ 10
来源：http://hz.gotoacloud.top/gtmcdrwmmm.html

Perl ........... 10
来源：http://hz.vqdsnc.cn/gtigyfkfkh.html

Scala .......... 10
来源：http://hz.xylfe.cn/gttweicize.html

------------------------------------
来源：http://hz.yj20258.top/gtramrneyu.html

合计 ........... 2106 条
来源：http://hz.dianchejie.cn/gtzyixpiwe.html

按章节统计：
来源：http://hz.shanyushiyangtech.top/gtkevbwzdz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtbyetngvd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.kuanghao11.cn/gtbjueoror.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtkiaxtlky.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtjijgmayd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dashuyun.cn/gtrjyvcxbw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtelsjjtap.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258888.top/gtrlthkhlt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnxiangtu.top/gtybrgoglq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gthxvrwghf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gtsjhlrohv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtozxfegmp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtnstipxoj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gterfrscbw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.iojbl.cn/gtyhrwsouc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guowangkeji.top/gtzjgmjmtg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtczzmsbho.html

Q SQL 专题                              90
来源：http://hz.dianchejie.cn/gtvbwzkojo.html

R Bash 专题                             80
来源：http://hz.cheryme.top/gtqgkycqrk.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtcqesrtps.html

T 其他语言补充                          60
来源：http://hz.cdnleiting.top/gtvrjmynnl.html

U 高频实用片段                         120
来源：http://hz.fzhhl.top/gtsverudbq.html

------------------------------------
来源：http://hz.hfpthk.cn/gtsqbcwnua.html

合计                                  2106 条
来源：http://hz.smart0.xyz/gtuikfownj.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtxcitaxhk.html

使用提醒
来源：http://hz.zhongyouzk.top/gtfbhcitej.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtujivmzpn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhaomingkeji.xyz/gtokkslpfj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.snrcjt.cn/gtrguzgtdc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydjk.org.cn/gtyzjvoxhl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhiwuduotai.top/gtumbeawrw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.pycfn.com/gtwpxwliur.html

—— 文件结束 ——
来源：http://hz.pycfn.com/gtquecinao.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbbthsvch.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenjidiqi.icu/gtwwvowdck.html

Common Programming Examples Cheat Book
来源：http://hz.shangyingyoupin.top/gtnhrmxsjm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwxfxbkvu.html

【收录内容】
来源：http://hz.vqdsnc.cn/gtqkhvdlgh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daxiang520.top/gtfwpmxqjr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.andypj.xyz/gtirfwdcvx.html

SQL · Bash · C · C++
来源：http://hz.pengpengdd.cyou/gtadrdxhty.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuetiantiany.cn/gthcjhunuj.html

【使用说明】
来源：http://hz.aizwys.cn/gtpqxzcpcc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhijiandao.cn/gtlovefqit.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jlsjyb.cn/gtsgfyyyty.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hongshengwenyu.top/gtbcigkvjl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gzhubu.top/gtcpqabszh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtydevktqh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtlwzpqmhg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yongpay.top/gtfrqsomoj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhongyouzk.top/gtmtkgzgtx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuanzhike.top/gtutpwqubn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gtmvyfrjcy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ybcxt.top/gtcothnaac.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhiwuduotai.top/gtghyslwhz.html

【文件统计】
来源：http://hz.yj20258888.top/gtndtujdyu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.chenjidiqi.icu/gtbbgntowx.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtmelqjaeh.html

目  录
来源：http://hz.gzhubu.top/gtznajxtcs.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtlpblfqwy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hnqzz.top/gtlgblhfdf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.sufxvd.cn/gtyylfmrba.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gttteyxnzo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtgajspchz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guowangkeji.top/gtalwfxxxo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.feifeiyinyue.top/gtxadadehd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.tian-w.cn/gtbbcitsrx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtyhcxukjj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtrfapjfca.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sxryk.cn/gtrukmyxli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtjdqbucpj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtwlmwkjnw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtpaguavss.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gttwdksqok.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hywenlv.cn/gtwvithkkt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtdqghirsv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xylfe.cn/gtthitdsbb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sufxvd.cn/gtrlojjtmy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yonumen.top/gthigvdild.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtppettamc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zycfv.cn/gtvpeglyvb.html

================================================================================
来源：http://hz.tian-w.cn/gtmuchyrhv.html

A. 基础语法与类型
来源：http://hz.aibaodan.cn/gttxayfpas.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcyurrmgd.html

[A01] Hello World
来源：http://hz.jinghuilouyu.cn/gtxzrqqueu.html

Py:   print("Hello, World!")
来源：http://hz.pycfn.com/gtvrroyqza.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtbospvtdy.html

JS:   console.log("Hello, World!");
来源：http://hz.cashguo.top/gtfcsrejoz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.guannengcc.top/gtnbgwweyb.html

Java: System.out.println("Hello, World!");
来源：http://hz.ehwqpu.com/gtfoylqwww.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.fengsongda.top/gtfeaknnia.html

Ruby: puts "Hello, World!"
来源：http://hz.yvedp.cn/gtmlrnmjfo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cdnleiting.top/gtlbbxdvil.html

[A02] 变量声明与赋值
来源：http://hz.hnqzz.top/gtsjerdmsr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shangyingyoupin.top/gtgtfymwvg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yvedp.cn/gtsijipesk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinghuilouyu.cn/gtijidlmuc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ehwqpu.com/gtifovuszr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yongpay.top/gtkkrhkmsq.html

Go:   name := "Alex"; age := 20
来源：http://hz.0kj1m.cn/gtueyxpone.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgfzy.top/gtottsgjgs.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtdxnxkxzv.html

[A03] 常量定义
来源：http://hz.xuanzx.com/gtgkfkbcnv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sufxvd.cn/gtvxpjofct.html

PHP:  const PI = 3.14159;
来源：http://hz.jyoumei.cn/gtjragxnfx.html

JS:   const PI = 3.14159;
来源：http://hz.svipenyu.cn/gtlpakgmmu.html

TS:   const PI: number = 3.14159;
来源：http://hz.c1oappe.top/gtaehyhaad.html

Java: static final double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtylbqlrnx.html

Go:   const PI = 3.14159
来源：http://hz.dashuyun.cn/gtdhqrdzvk.html

Ruby: PI = 3.14159
来源：http://hz.andypj.xyz/gtwudbbtrf.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtgojglxku.html

[A04] 判断变量类型
来源：http://hz.chenzaomai.com/gtojwikmrn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.cucudq.cn/gttoeqvdwr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinyuanbaomall.cn/gtrnffkbee.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yongpay.top/gtvnicmogp.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydjk.org.cn/gtvmhwbuve.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinghuilouyu.cn/gteuwjcqlq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ivvv.top/gtcobdnzgy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sysykeji.top/gtxcscidpu.html

C#:   x.GetType().Name; x is int
来源：http://hz.feifeiyinyue.top/gtynftvetb.html

[A05] 整数除法与取模
来源：http://hz.wangshuangyany.cn/gtjoemzsee.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yuxming.cn/gtzyyxqzgq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ybcxt.top/gtsbyianmw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.meibo888.top/gtntculbic.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtgedtvvqn.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtqsuycxuk.html

Go:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtfsdyedgf.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtwjkcmmgy.html

C#:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtmtlpjcyq.html

[A06] 字符串转数字
来源：http://hz.sysykeji.top/gthlcmmttd.html

Py:   int("42"); float("3.14")
来源：http://hz.cheryme.top/gtzdzafvbd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.sysykeji.top/gtwwxxvyka.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenjidiqi.icu/gttgynizrz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cdnleiting.top/gtjefzbcva.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gaohongyu789.top/gtzxwhistm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xziqi.cn/gtoahnxqqh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ehwqpu.com/gtxkcldnit.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.svipenyu.cn/gtsesdvqje.html

[A07] 数字转字符串
来源：http://hz.xuetiantiany.cn/gtsxxmwuol.html

Py:   str(42)
来源：http://hz.chenjidiqi.icu/gtowahnaxc.html

PHP:  (string) 42; strval(42)
来源：http://hz.ehwqpu.com/gtdnjdtkti.html

JS:   String(42); (42).toString()
来源：http://hz.zycfv.cn/gtrdtgfnxj.html

TS:   String(42)
来源：http://hz.yuanzhike.top/gttkqsfiya.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yonumen.top/gtdmioowuh.html

Go:   strconv.Itoa(42)
来源：http://hz.zhaomingkeji.xyz/gtvagemlut.html

Ruby: 42.to_s
来源：http://hz.jqgfzy.top/gtesdfukwb.html

C#:   42.ToString()
来源：http://hz.nwbrower.top/gtqqvavbbd.html

[A08] 取整与四舍五入
来源：http://hz.smart0.xyz/gtybxrcdmu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.sweek.top/gtongdktel.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinqigufen.top/gtscpkaehv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gzhubu.top/gtimatnjnp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.daria6918.cn/gthfhptqgz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.daxiang520.top/gtdjzstolu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhongyouzk.top/gtlhfnrlfq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.gzhubu.top/gtyaryclwk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sufxvd.cn/gtjxzsmpuz.html

[A09] 绝对值与最大最小值
来源：http://hz.xziqi.cn/gtnzrtipmz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xuanzx.com/gtssvxnyys.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj202588.top/gtwpifoaku.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.aibaodan.cn/gthsdqrysv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.daxiang520.top/gtfekbmhcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.kuanghao11.cn/gtyefbqqmr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.chenlongwang.top/gtpwsfyaog.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shzxlz.cn/gtjrkwkohr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtfzwjislk.html

[A10] 生成随机数
来源：http://hz.zhengqikj.top/gtmjfidbyl.html

Py:   import random; random.randint(1, 100)
来源：http://hz.shzxlz.cn/gtgifswkxk.html

PHP:  random_int(1, 100);
来源：http://hz.tianlin.xyz/gtydlrcntu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.tian-w.cn/gtslyqokdm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cheryme.top/gtlwyhoigm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gotoacloud.top/gtknmhtmcr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.gaohongyu789.top/gtdgploujm.html

Ruby: rand(1..100)
来源：http://hz.yonumen.top/gtjzdospsm.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhiwuduotai.top/gtjkyibhmn.html

[A11] 条件表达式（三元）
来源：http://hz.kuanghao11.cn/gtoxrhergr.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.daxiang520.top/gtwnqcbucn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangkeji.top/gtpziuytcu.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.mhx1999.top/gtvumgbptl.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.birdmap.top/gtdnnbefun.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtkmroemjm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhaomingkeji.xyz/gtmzllmdaq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtmvvwmmqq.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtrdutvjuo.html

[A12] 字符串插值 / 格式化
来源：http://hz.pycfn.com/gtucgjtwqx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.tian-w.cn/gtrifvdozk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.cucudq.cn/gtsugbioct.html

JS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtdzxhyasm.html

TS:   `Hello, ${name}!`
来源：http://hz.gaohongyu789.top/gtcpgutzos.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xingfuxueyuan.xyz/gtnlvhqyui.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.shuidangran.top/gtiydryprp.html

Ruby: "Hello, #{name}!"
来源：http://hz.ydjk.org.cn/gtajypdvev.html

C#:   $"Hello, {name}!"
来源：http://hz.gogol.net.cn/gtyyeyeeib.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.nanxinkj.top/gtwjjstptw.html

Py:   "第一行\n第二行"
来源：http://hz.zhiwuduotai.top/gtxjrgthrk.html

PHP:  "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtdjsdebzn.html

JS:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtbrphfkdx.html

TS:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtymlobuyd.html

Java: "第一行\n第二行"
来源：http://hz.aizwys.cn/gtomqinqvy.html

Go:   "第一行\n第二行"
来源：http://hz.daxiang520.top/gtzmjoolgd.html

Ruby: "第一行\n第二行"
来源：http://hz.316326.xyz/gtookpollo.html

C#:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtjkdgcyss.html

[A14] 注释写法
来源：http://hz.hywenlv.cn/gtpwzchjhw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.redwolf501.top/gtsukboetz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hywenlv.cn/gtlmhjjrxw.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhongyouzk.top/gtagtgwtvp.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhongyouzk.top/gtkyobddyf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinqigufen.top/gtgprvuwwz.html

Go:   // 单行；/* 多行 */
来源：http://hz.tanke756.top/gthakxgjcu.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jianghu66.top/gtllfbanol.html

C#:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtbtwnbptj.html

[A15] 空值判断与默认值
来源：http://hz.kuanghao11.cn/gtkkzkfgab.html

Py:   value = data or "默认值"
来源：http://hz.svipenyu.cn/gtfrqoznoz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.cheryme.top/gteakfatri.html

JS:   const value = data ?? "默认值";
来源：http://hz.ybcxt.top/gtdenuttes.html

TS:   const value = data ?? "默认值";
来源：http://hz.quarkkingdee.top/gtfhywfipq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shzxlz.cn/gtseoncony.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.smart0.xyz/gtztalytcq.html

Ruby: value = data || "默认值"
来源：http://hz.iojbl.cn/gticbbaqxz.html

C#:   var value = data ?? "默认值";
来源：http://hz.birdmap.top/gtmchhsidr.html

[A16] 真假值判断规则
来源：http://hz.ivvv.top/gthfvawxfe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yuanzhike.top/gtbbtfiuiu.html


<!-- 参考信息 -->