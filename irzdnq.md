代发 wailian999

[U89] JS：数组去重
来源：http://hz.xylfe.cn/gtpmkcnnnc.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gthvomwqir.html

[U90] JS：数字数组排序
来源：http://hz.mhx1999.top/gtxihwrrgk.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtobgwhwgh.html

[U91] JS：对象键值遍历
来源：http://hz.svipenyu.cn/gtmsnkpkib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cucudq.cn/gthtljnnnq.html

[U92] JS：深拷贝
来源：http://hz.hysaishi.cn/gtqgohfefb.html

structuredClone(obj)
来源：http://hz.zhengqikj.top/gtvfwpglag.html

[U93] JS：模板字符串
来源：http://hz.xuanzx.com/gtqsqjduao.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtswwtcwqz.html

[U94] JS：箭头函数
来源：http://hz.jinyuanbaomall.cn/gtxblhefqp.html

const double = x => x * 2;
来源：http://hz.shanyushiyangkeji.top/gtmjfxckhe.html

[U95] JS：Promise 包装
来源：http://hz.wangdashe.top/gtowzighkc.html

new Promise((resolve, reject) => {})
来源：http://hz.dashuyun.cn/gtcouvqvhp.html

[U96] JS：async/await 与异常
来源：http://hz.yuxming.cn/gtlwfsamsl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gthgrfamzi.html

[U97] JS：并发请求
来源：http://hz.pycfn.com/gtgsfzeeqn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtlqzjauvs.html

[U98] JS：fetch 带 JSON
来源：http://hz.cucudq.cn/gtsezgyglt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtwnqdhase.html

[U99] JS：事件监听
来源：http://hz.cashguo.top/gthhbyapei.html

el.addEventListener("click", e => {})
来源：http://hz.jinqigufen.top/gtysuesqve.html

[U100] JS：DOM 查询
来源：http://hz.gzhubu.top/gtorhaqywx.html

document.querySelector(".item")
来源：http://hz.ppjwa.cn/gtodusvqdk.html

[U101] JS：classList 操作
来源：http://hz.jinqigfzy.top/gtmawbbavs.html

el.classList.toggle("active")
来源：http://hz.zdqjudy.top/gtpknqldbz.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gteoublfsc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.daxiang520.top/gtwhjxdpmt.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtyaskrgmd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.smart0.xyz/gtohegowxu.html

[U104] JS：防抖
来源：http://hz.chenlongwang.top/gtfwpxfmvc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtdhpxijwc.html

[U105] JS：节流
来源：http://hz.hywenlv.cn/gthccfekme.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xylfe.cn/gtaffuwmxk.html

[U106] JS：日期格式化
来源：http://hz.xinyue.icu/gtmkirglla.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guannengcc.top/gtuysbmvei.html

[U107] JS：数字千分位
来源：http://hz.tianlin.xyz/gthlittmcw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gtgskieomi.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gthnsjmppd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258888.top/gtzvktrfzi.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtsircrvzn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtgyrexwgq.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtwsmgvtuv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gogol.net.cn/gtkmggjzab.html

[U111] JS：对象转 Map
来源：http://hz.yonumen.top/gtcirxnxuv.html

new Map(Object.entries(obj))
来源：http://hz.aibaodan.cn/gtalfqomyw.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtyrukscuc.html

"7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gthprdvixx.html

[U113] JS：正则替换全部
来源：http://hz.ehwqpu.com/gttnwugzoc.html

s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtcafwgxmk.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtkenwhduy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtpvcuiwgq.html

[U115] JS：生成 UUID
来源：http://hz.jinghuilouyu.cn/gtzcybegfl.html

crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtklvjrhxx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tanke756.top/gtdxtbvzrp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtzszbuvjq.html

[U117] JS：单元测试
来源：http://hz.tianlin.xyz/gtqauxjidu.html

npm i -D vitest;  npx vitest
来源：http://hz.shuidangran.top/gtafcmhoyi.html

[U118] JS：开发服务器
来源：http://hz.hywenlv.cn/gtvtdgfica.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gtfamjupfp.html

[U119] JS：生产构建
来源：http://hz.jqgufenzy.top/gtrtqwenve.html

npx vite build
来源：http://hz.hnxiangtu.top/gtzrawgssg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sufxvd.cn/gtzzmxqaiw.html

import.meta.env.VITE_API_URL
来源：http://hz.xziqi.cn/gtsitwlcdz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtserjiszk.html

统计汇总
来源：http://hz.jyoumei.cn/gtgjjmptdj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkrgvtfna.html

按语言统计（条）：
来源：http://hz.nwbrower.top/gtyazkuhtc.html

Python ......... 252
来源：http://hz.shzxlz.cn/gtdwataesx.html

PHP ............ 252
来源：http://hz.xziqi.cn/gtpbgvjrzj.html

JavaScript ..... 252
来源：http://hz.xylfe.cn/gtgwfkcdow.html

TypeScript ..... 212
来源：http://hz.nanxuanxn.top/gtrvotusqc.html

Java ........... 212
来源：http://hz.jiagoushi.top/gtpvjkiuaa.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gtfmdjihdk.html

Ruby ........... 212
来源：http://hz.jyoumei.cn/gtzvmhcxyy.html

C# ............. 212
来源：http://hz.xingfuxueyuan.xyz/gtczmqrwnb.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtdeqbrdlf.html

C++ ............ 30
来源：http://hz.nwbrower.top/gtquryxowv.html

SQL ............ 90
来源：http://hz.xingfuxueyuan.xyz/gtroonnrbz.html

Bash ........... 80
来源：http://hz.yvedp.cn/gtqzjnrjmc.html

Kotlin ......... 15
来源：http://hz.havefunace.top/gtxpbnsnxx.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtkaaqqnsr.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtqrcvwhgw.html

Perl ........... 10
来源：http://hz.snrcjt.cn/gtmrmorjsh.html

Scala .......... 10
来源：http://hz.yonumen.top/gtvlnzurdt.html

------------------------------------
来源：http://hz.xziqi.cn/gtnsbhuthu.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtfefdbses.html

按章节统计：
来源：http://hz.cdnleiting.top/gtbzltmshe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtohjiyryl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtuejxdimn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtdnthkzws.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtlloydyup.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zycfv.cn/gtsujzlvup.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gteoyfgiha.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gthblxpzjh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtxhstlotd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtvjamsbzj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gogol.net.cn/gtcjnxsvyz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtgbpcfcsl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtssremdhy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtsucbthny.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtyktoxdvk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.snrcjt.cn/gteamjpmsg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtjtchqqpm.html

Q SQL 专题                              90
来源：http://hz.yuanzhike.top/gtxkdnveuu.html

R Bash 专题                             80
来源：http://hz.shangyingyoupin.top/gthrqdvyfn.html

S C / C++ 专题                          60
来源：http://hz.daria6918.cn/gtdpxzbgsh.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtgczwjaad.html

U 高频实用片段                         120
来源：http://hz.guannengcc.top/gtymqekjnf.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtxbsbilpn.html

合计                                  2106 条
来源：http://hz.316326.xyz/gthddiivmj.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtnzaclqmq.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtrizgtsys.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gticmrbfrz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.c1oappe.top/gtesmqjnxw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cqqwz.cn/gtklabmxyh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shzxlz.cn/gtxmlptplg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.vqdsnc.cn/gtrxquoial.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cashguo.top/gtzwxcepwa.html

—— 文件结束 ——
来源：http://hz.yvedp.cn/gtodvwsenk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsjlosdoz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinghuilouyu.cn/gtgcgykaxl.html

Common Programming Examples Cheat Book
来源：http://hz.yj20258888.top/gtlagkvrkm.html

================================================================================
来源：http://hz.dashuyun.cn/gtvhsokton.html

【收录内容】
来源：http://hz.shangyingyoupin.top/gtmyaysoye.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.316326.xyz/gtylykxwms.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhoulong.xyz/gtzttgaboz.html

SQL · Bash · C · C++
来源：http://hz.ivvv.top/gtuppjxupw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj202588.top/gtyicjljcg.html

【使用说明】
来源：http://hz.zhixingplan.top/gtnvargsbp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cqqwz.cn/gtepqfijws.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xinyue.icu/gtlzfkfmel.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hammf.cn/gtlpzewejm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ppjwa.cn/gtgddfarbc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ybcxt.top/gtyhlhvfgf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xylfe.cn/gttzzwjbjh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xinyue.icu/gtbeeshsxs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtfdmgrdrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cdnleiting.top/gtvhyohpxl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.redwolf501.top/gtlkbkacoo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.fengsongda.top/gtcvgccxpu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nanxuanxn.top/gtcjgvdycn.html

【文件统计】
来源：http://hz.yongpay.top/gtjhcdfohx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dashuyun.cn/gtxzljudpf.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtghhjgzuq.html

目  录
来源：http://hz.hongshengwenyu.top/gtkgucdldo.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gttizisxzj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenjidiqi.icu/gtzwcsedra.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtorldekhg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gthwpxcktp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gtggvqhdun.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shuidangran.top/gtzzsqsklf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtppplywtb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gtjogsjhjv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtlsjdmqud.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtedtzomvt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cucudq.cn/gtbyedzfjf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtuprupszb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gtnfhdjjja.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtmwfjwbvy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tianlin.xyz/gtlydlrptv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258.top/gtbqbtukxh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtvaykpdcw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fengsongda.top/gtsjppazji.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jlsjyb.cn/gtsvhfgzuc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hfpthk.cn/gtwguptkdb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtpmperxwb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtwzssqdsn.html

================================================================================
来源：http://hz.ivvv.top/gtnrxyrhmv.html

A. 基础语法与类型
来源：http://hz.jianghu66.top/gturxuxwjd.html

================================================================================
来源：http://hz.tianlin.xyz/gtkcvmervp.html

[A01] Hello World
来源：http://hz.shangyingyoupin.top/gtgjrybavk.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtunospfnc.html

PHP:  echo "Hello, World!";
来源：http://hz.cdnleiting.top/gtisxracpy.html

JS:   console.log("Hello, World!");
来源：http://hz.aibaodan.cn/gtbxrlywcs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj202588.top/gtwyxamxgy.html

Java: System.out.println("Hello, World!");
来源：http://hz.ehwqpu.com/gtnktmifoe.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hammf.cn/gthltrdzhs.html

Ruby: puts "Hello, World!"
来源：http://hz.cashguo.top/gtmofqigol.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jiagoushi.top/gtxptbkpia.html

[A02] 变量声明与赋值
来源：http://hz.andypj.xyz/gtwxtgzrct.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhaomingkeji.xyz/gtckormfcl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.wangshuangyany.cn/gtanhsryff.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gotoacloud.top/gtxtrgimwy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.nwbrower.top/gtybvhwqaz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhaomingkeji.xyz/gtkiogxwve.html

Go:   name := "Alex"; age := 20
来源：http://hz.jyoumei.cn/gtdjggkfsn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gtuxwsyqer.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtncphzmat.html

[A03] 常量定义
来源：http://hz.hammf.cn/gtjnsnqswl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.redwolf501.top/gtpyguovjw.html

PHP:  const PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gteooplfan.html

JS:   const PI = 3.14159;
来源：http://hz.jqgfzy.top/gttumklxvd.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuanzhike.top/gtqdtowwsx.html

Java: static final double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtiexdwfks.html

Go:   const PI = 3.14159
来源：http://hz.iojbl.cn/gtwcnbdcgz.html

Ruby: PI = 3.14159
来源：http://hz.9152youxi.cn/gtfjipvoyb.html

C#:   const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtzcagyltx.html

[A04] 判断变量类型
来源：http://hz.yj20258.top/gtqyvwbbcp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhiwuduotai.top/gttswsspgl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.quarkkingdee.top/gtpwxpwwzg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.guannengcc.top/gtjwontxho.html

TS:   typeof x; x instanceof Date
来源：http://hz.pengpengdd.cyou/gtdfqqofgl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ydjk.org.cn/gtzxuvglup.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.chenzaomai.com/gtyboswzcy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jqgufenzy.top/gtdgnndujo.html

C#:   x.GetType().Name; x is int
来源：http://hz.sweek.top/gtzhuqieum.html

[A05] 整数除法与取模
来源：http://hz.hnxiangtu.top/gtsoehbjgg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.meibo888.top/gtffrortok.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.316326.xyz/gtllnpbplg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hfpthk.cn/gtaudeqzte.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtqihkhflk.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gthqdvysri.html

Go:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtuzrmqygj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtkztatbdw.html

C#:   7 / 2; 7 % 2
来源：http://hz.0kj1m.cn/gtczaslekv.html

[A06] 字符串转数字
来源：http://hz.yj20258888.top/gtsdowhxli.html

Py:   int("42"); float("3.14")
来源：http://hz.jqgfzy.top/gtzsibsszj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.nanxuanxn.top/gtkqnnlweq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.fengsongda.top/gtwejgvghi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shanyushiyangtech.top/gtibigummr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cdnleiting.top/gtkgbslhhi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jyoumei.cn/gtksrqxvul.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.kuanghao11.cn/gtixhcqynq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gotoacloud.top/gtgxykciwp.html

[A07] 数字转字符串
来源：http://hz.sweek.top/gtivpxxptx.html

Py:   str(42)
来源：http://hz.chenzaomai.com/gtzwqxfqjz.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj20258.top/gtfbhlcwko.html

JS:   String(42); (42).toString()
来源：http://hz.haohaochexian.top/gtytynnyoj.html

TS:   String(42)
来源：http://hz.fzhhl.top/gtghekcabw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.aibaodan.cn/gtxquwhbbh.html

Go:   strconv.Itoa(42)
来源：http://hz.fengsongda.top/gtmxemizrm.html

Ruby: 42.to_s
来源：http://hz.zycfv.cn/gtedtegjlh.html

C#:   42.ToString()
来源：http://hz.jqgufenzy.top/gthtrvqres.html

[A08] 取整与四舍五入
来源：http://hz.fengsongda.top/gtlsoehywf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shuidangran.top/gtsieyoqwg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinqigfzy.top/gtjfkcvolf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.snrcjt.cn/gtflupisky.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hywenlv.cn/gtvtnrtjyu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yuxming.cn/gtjalultwr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhixingplan.top/gtmvdkuglm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.pengpengdd.cyou/gtohpvijcq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sxryk.cn/gtrilgaumh.html

[A09] 绝对值与最大最小值
来源：http://hz.mhx1999.top/gtlvqwswel.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hongshengwenyu.top/gtcdctswfs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuanzhike.top/gtapqagzsx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.smart0.xyz/gtspysxkyx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigfzy.top/gtgwfswrmg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hfpthk.cn/gtqizkxmms.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.sweek.top/gtzhxgmgfe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.sweek.top/gtyvhcqtke.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenzaomai.com/gtjgfagbnb.html

[A10] 生成随机数
来源：http://hz.meibo888.top/gtslhfnlxs.html

Py:   import random; random.randint(1, 100)
来源：http://hz.fzhhl.top/gtozesifkf.html

PHP:  random_int(1, 100);
来源：http://hz.guannengcc.top/gtjqmoawmm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhengqikj.top/gtcmuovnjy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj202588.top/gtddgawhus.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cucudq.cn/gtxqekjles.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.chenzaomai.com/gtghpzqabx.html

Ruby: rand(1..100)
来源：http://hz.gzhubu.top/gthccbqyhu.html

C#:   new Random().Next(1, 101)
来源：http://hz.fengsongda.top/gtxtvwajof.html

[A11] 条件表达式（三元）
来源：http://hz.snrcjt.cn/gttwdqdosd.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.meibo888.top/gtelhhvfyd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtbhyxekdz.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtajkxhayx.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtnsrvrwwn.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtarzlcyvx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhoulong.xyz/gtqyufncwp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtnlqoanhb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gtbdycwvri.html

[A12] 字符串插值 / 格式化
来源：http://hz.0kj1m.cn/gtkhyrpzrv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.sweek.top/gtoerjyyaq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhiwuduotai.top/gtlahurvtb.html

JS:   `Hello, ${name}!`
来源：http://hz.ybcxt.top/gtfieqsyhu.html

TS:   `Hello, ${name}!`
来源：http://hz.daxiang520.top/gtfdkxhwin.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.wangdashe.top/gtlgspbtmz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinqigfzy.top/gtqyvtqcag.html

Ruby: "Hello, #{name}!"
来源：http://hz.zhaomingkeji.xyz/gtnwmgyajw.html

C#:   $"Hello, {name}!"
来源：http://hz.316326.xyz/gtplmfmngp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jinghuilouyu.cn/gtutgraszl.html

Py:   "第一行\n第二行"
来源：http://hz.redwolf501.top/gtudfbobhr.html

PHP:  "第一行\n第二行"
来源：http://hz.xuanzx.com/gtccijriwy.html

JS:   "第一行\n第二行"
来源：http://hz.yonumen.top/gtsodarhga.html

TS:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtxdubobfv.html

Java: "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtettqmrdu.html

Go:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtpoyrqlgi.html

Ruby: "第一行\n第二行"
来源：http://hz.havefunace.top/gtbwnptepr.html

C#:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtswwhmpks.html

[A14] 注释写法
来源：http://hz.0kj1m.cn/gtogeftcww.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yuanzhike.top/gtemdovdnl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtymbefuvc.html

JS:   // 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtgvlortqo.html

TS:   // 单行；/* 多行 */
来源：http://hz.cheryme.top/gtdmvudozb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.smart0.xyz/gtuwpwtkss.html

Go:   // 单行；/* 多行 */
来源：http://hz.yvedp.cn/gtqnvhzzjs.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.guowangkeji.top/gtcuzllavy.html

C#:   // 单行；/* 多行 */
来源：http://hz.cucudq.cn/gtgkehhynd.html

[A15] 空值判断与默认值
来源：http://hz.snrcjt.cn/gtyhkivkdk.html

Py:   value = data or "默认值"
来源：http://hz.ydzc1.top/gtfcvcrytc.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xziqi.cn/gtjnpntdzx.html


<!-- 参考信息 -->