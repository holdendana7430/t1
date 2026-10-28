代发 wailian999

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gtgmvkrnbj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhengqikj.top/gtqkgiyhgf.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gtrogutoyq.html

{ ...a, ...b }
来源：http://hz.dashuyun.cn/gtjbtxsihn.html

[U89] JS：数组去重
来源：http://hz.zhengqikj.top/gtsaiwgsng.html

[...new Set(arr)]
来源：http://hz.gotoacloud.top/gtgszswjzw.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangtech.top/gtcyiqqrep.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtqleecjha.html

[U91] JS：对象键值遍历
来源：http://hz.0kj1m.cn/gtxiotjrtp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sxryk.cn/gtzydrmfeh.html

[U92] JS：深拷贝
来源：http://hz.zhengqikj.top/gtortacpik.html

structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtmrzlzilr.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtfygllgke.html

`共 ${n} 条`
来源：http://hz.shuidangran.top/gtfwicxzlp.html

[U94] JS：箭头函数
来源：http://hz.yj202588.top/gtpijlpquw.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gtxuwgqinh.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangkeji.top/gtqwmjbwfr.html

new Promise((resolve, reject) => {})
来源：http://hz.jiagoushi.top/gtmcplijwy.html

[U96] JS：async/await 与异常
来源：http://hz.shangyingyoupin.top/gtqiezhhnd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gthcjglmis.html

[U97] JS：并发请求
来源：http://hz.cucudq.cn/gtssgstdib.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtmejbxzqk.html

[U98] JS：fetch 带 JSON
来源：http://hz.quarkkingdee.top/gtcdxjsrpy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ywan-chungtsiang.top/gtzlbuufnd.html

[U99] JS：事件监听
来源：http://hz.jyoumei.cn/gtuuzwdjsm.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gtzorfmscc.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtygfjhmyp.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gtndycccuj.html

[U101] JS：classList 操作
来源：http://hz.zhaomingkeji.xyz/gtvpesrbdc.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtzuyqznbv.html

[U102] JS：本地存储
来源：http://hz.chenzaomai.com/gtajpdmnue.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtunulmhgx.html

[U103] JS：定时器
来源：http://hz.ivvv.top/gtpoqaypfn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuetiantiany.cn/gtrlftsgpl.html

[U104] JS：防抖
来源：http://hz.zhengqikj.top/gteegaiqif.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtoryhdfeb.html

[U105] JS：节流
来源：http://hz.havefunace.top/gtxkbqpxtz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.haohaochexian.top/gtbacuxevl.html

[U106] JS：日期格式化
来源：http://hz.ppjwa.cn/gtjwaovfnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sxryk.cn/gtwqjkxoux.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtrcziduzj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.bjfxy.top/gtmnowencp.html

[U108] JS：随机整数
来源：http://hz.tian-w.cn/gtqmtmbsdw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jianghu66.top/gtuplrxxxw.html

[U109] JS：数组分组
来源：http://hz.yangfankeji.com/gtglwjkevw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtdtbqgqao.html

[U110] JS：数组分块
来源：http://hz.sweek.top/gtctdpylqz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cqqwz.cn/gtxmpskcik.html

[U111] JS：对象转 Map
来源：http://hz.iojbl.cn/gtpnmsjypj.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gtuwtcotbu.html

[U112] JS：字符串补位
来源：http://hz.nwbrower.top/gtherdicly.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtzirryhlj.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtpungodjc.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtpmywfktn.html

[U114] JS：JSON 深比较
来源：http://hz.zhoulong.xyz/gtydglgsbh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtqapmsxoc.html

[U115] JS：生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtppbsmyhl.html

crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtdybjcqeq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jqgfzy.top/gtfbikhyqm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cashguo.top/gtxuxmmzwy.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gtbhrndmcz.html

npm i -D vitest;  npx vitest
来源：http://hz.jinghuilouyu.cn/gtfeghvxog.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtzaxagdhb.html

npm i -D vite;  npx vite
来源：http://hz.jqgufenzy.top/gtojqjrrvg.html

[U119] JS：生产构建
来源：http://hz.zhongyouzk.top/gtxwwgfags.html

npx vite build
来源：http://hz.yongpay.top/gtcgmfwjtj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenlongwang.top/gtttlwpjxs.html

import.meta.env.VITE_API_URL
来源：http://hz.wangdashe.top/gtrmwrupaz.html

================================================================================
来源：http://hz.ehwqpu.com/gtcnhlqsqc.html

统计汇总
来源：http://hz.svipenyu.cn/gtefaadfnn.html

================================================================================
来源：http://hz.aizwys.cn/gtaxgqzmak.html

按语言统计（条）：
来源：http://hz.xziqi.cn/gtggnphtxc.html

Python ......... 252
来源：http://hz.ivvv.top/gtuaumfghd.html

PHP ............ 252
来源：http://hz.gogol.net.cn/gtugioznhf.html

JavaScript ..... 252
来源：http://hz.xingfuxueyuan.xyz/gtgapspqkt.html

TypeScript ..... 212
来源：http://hz.hammf.cn/gtytxslpjl.html

Java ........... 212
来源：http://hz.gaohongyu789.top/gtpfxvjhaq.html

Go ............. 212
来源：http://hz.ivvv.top/gtgrcyqlmu.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtigodigbu.html

C# ............. 212
来源：http://hz.jqgfzy.top/gthvresebz.html

C .............. 30
来源：http://hz.jiagoushi.top/gtooqsrtzt.html

C++ ............ 30
来源：http://hz.xinyue.icu/gtapxvginw.html

SQL ............ 90
来源：http://hz.yonumen.top/gttccdtudf.html

Bash ........... 80
来源：http://hz.jinqigfzy.top/gtmgfuoojd.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtzkrtnnsh.html

Swift .......... 15
来源：http://hz.fengsongda.top/gtwxxgapmx.html

Lua ............ 10
来源：http://hz.snrcjt.cn/gtyakhohzh.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gtobjxukoy.html

Scala .......... 10
来源：http://hz.daria6918.cn/gtziwizwqz.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtheeedyij.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gthiynxbjy.html

按章节统计：
来源：http://hz.fzhhl.top/gtskdamsmx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgufenzy.top/gtklklareq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtivalekqj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtoclvmjwk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtsccjuxbb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sweek.top/gtxzlydslc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtbfxqaroz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtjrwkwkkl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtmhzzicef.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtmifyzsoz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtpatslpou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtmuugbxiu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtvsglfmkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtcljwpkns.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtsoqukjza.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yongpay.top/gtognjfsot.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtypdwbudm.html

Q SQL 专题                              90
来源：http://hz.hysaishi.cn/gtfdjkllrx.html

R Bash 专题                             80
来源：http://hz.cucudq.cn/gtyajlpizs.html

S C / C++ 专题                          60
来源：http://hz.zhiwuduotai.top/gtcizpzmoh.html

T 其他语言补充                          60
来源：http://hz.hfpthk.cn/gtceneuqgq.html

U 高频实用片段                         120
来源：http://hz.jinqigfzy.top/gtkondsame.html

------------------------------------
来源：http://hz.ivvv.top/gtcjighgol.html

合计                                  2106 条
来源：http://hz.redwolf501.top/gtnkkkmolm.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtlgmealrr.html

使用提醒
来源：http://hz.sysykeji.top/gtykqsfbgi.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtfxvsxycb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jianghu66.top/gtrfavdnly.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hfpthk.cn/gtbnampdqi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hywenlv.cn/gtpjvficpp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fengsongda.top/gthmmobxyw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hysaishi.cn/gtzzqiudmm.html

—— 文件结束 ——
来源：http://hz.hammf.cn/gttkhkxmew.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsmpzutim.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cucudq.cn/gtgozaxafw.html

Common Programming Examples Cheat Book
来源：http://hz.haohaochexian.top/gtpexstqvr.html

================================================================================
来源：http://hz.cqqwz.cn/gtbaoiukbw.html

【收录内容】
来源：http://hz.nanxuanxn.top/gtekeuylci.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhoulong.xyz/gtnkjascfn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gtrpxbfrzb.html

SQL · Bash · C · C++
来源：http://hz.jiagoushi.top/gteonbudes.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jlsjyb.cn/gtxlkbkxyv.html

【使用说明】
来源：http://hz.hywenlv.cn/gthlqyhojw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.316326.xyz/gtbwferexd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hammf.cn/gtgdzniaog.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxinkj.top/gthmnopayw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hnqzz.top/gtxiojiyzt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtknhthgev.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj202588.top/gtppuvlcvy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj20258.top/gtcnrvyatc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ywan-chungtsiang.top/gtgcovodza.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj202588.top/gtwdrhdnbx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gaohongyu789.top/gtchjwwtbv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhaomingkeji.xyz/gtggblddcy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sysykeji.top/gthnqeihuc.html

【文件统计】
来源：http://hz.jianghu66.top/gtvxiswqkh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xylfe.cn/gtnjztufcw.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtldabhmlc.html

目  录
来源：http://hz.ywan-chungtsiang.top/gtltrnsvsl.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtbkobeeym.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.daria6918.cn/gtayrlirqg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtbqggtbaw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtttzhhpwr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jianghu66.top/gtohlkfhpp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dianchejie.cn/gtauolpiph.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.svipenyu.cn/gtsifwhhdg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtdvwelnaq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ydzc1.top/gthtpbsgso.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtovnvptoj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gttnqbzsog.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtjgukvean.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtegpgvhbo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtsuhwyqzd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jyoumei.cn/gtswlnrqso.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zdqjudy.top/gthiwtjuap.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtdwywlmbc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jlsjyb.cn/gtskmzxsfa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinqigufen.top/gtquumeekp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnqzz.top/gtgcluqcom.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtujdhunec.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ywan-chungtsiang.top/gtkvnwyltt.html

================================================================================
来源：http://hz.daxiang520.top/gtukssbqkn.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gtgbdhyrcy.html

================================================================================
来源：http://hz.pycfn.com/gttqwxzzge.html

[A01] Hello World
来源：http://hz.ybcxt.top/gthxcutofe.html

Py:   print("Hello, World!")
来源：http://hz.gotoacloud.top/gtbhyfpnfw.html

PHP:  echo "Hello, World!";
来源：http://hz.cheryme.top/gtookeyjbl.html

JS:   console.log("Hello, World!");
来源：http://hz.jqgufenzy.top/gtnnzhbywg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.0kj1m.cn/gtdeysixcy.html

Java: System.out.println("Hello, World!");
来源：http://hz.yueranfly.top/gtinskiaaa.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.tianlin.xyz/gttbpkaxry.html

Ruby: puts "Hello, World!"
来源：http://hz.vqdsnc.cn/gtqpyzoskb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.svipenyu.cn/gthxiuhubq.html

[A02] 变量声明与赋值
来源：http://hz.dashuyun.cn/gtfcbejlht.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hammf.cn/gtjozidahn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gtitiuttug.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sufxvd.cn/gtwwyiqpxx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jiagoushi.top/gtdtackufv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yuxming.cn/gtzomaxoal.html

Go:   name := "Alex"; age := 20
来源：http://hz.birdmap.top/gtqjdongbv.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sxryk.cn/gtyspldsnw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtmnltwami.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtcxlhjudk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sweek.top/gtfcfrjmge.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258.top/gtgewyilgs.html

JS:   const PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtamkhloic.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhiwuduotai.top/gtxhodqums.html

Java: static final double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtustreuyc.html

Go:   const PI = 3.14159
来源：http://hz.aizwys.cn/gtppiefdbp.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtevjpnyaz.html

C#:   const double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtwyjderpn.html

[A04] 判断变量类型
来源：http://hz.hongshengwenyu.top/gtlfjhfiri.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yuxming.cn/gtymtbeqoi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jianghu66.top/gtiokvddia.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnxiangtu.top/gttxpmwrge.html

TS:   typeof x; x instanceof Date
来源：http://hz.cucudq.cn/gtzaagbvzo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinqigfzy.top/gtusonlzug.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yvedp.cn/gtlxdsoyjx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sxryk.cn/gtdrbwohag.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinyuanbaomall.cn/gtmbqgrqwf.html

[A05] 整数除法与取模
来源：http://hz.yj202588.top/gtmtazxblg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.haohaochexian.top/gtqhubmbqn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xinyue.icu/gtzzgajape.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gttqhzyojf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhixingplan.top/gttlhydiis.html

Java: 7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtqkmelhlx.html

Go:   7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtyivaffvl.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtqlkknrmg.html

C#:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gteqdxdojz.html

[A06] 字符串转数字
来源：http://hz.ydjk.org.cn/gtkjjlutvv.html

Py:   int("42"); float("3.14")
来源：http://hz.pengpengdd.cyou/gtzdkttbfj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gzhubu.top/gtvnkjctqb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.mhx1999.top/gtclafkxgp.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hnqzz.top/gtzdpifmxb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuxming.cn/gtcrfoofoy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.iojbl.cn/gtwpuoubng.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.haohaochexian.top/gtzghmgbqm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.smart0.xyz/gtnrgpopys.html

[A07] 数字转字符串
来源：http://hz.jlsjyb.cn/gtvukmtvap.html

Py:   str(42)
来源：http://hz.zhaomingkeji.xyz/gtvlezzlxr.html

PHP:  (string) 42; strval(42)
来源：http://hz.gogol.net.cn/gtijzefjqm.html

JS:   String(42); (42).toString()
来源：http://hz.dashuyun.cn/gttqfcrmlo.html

TS:   String(42)
来源：http://hz.zhiwuduotai.top/gtwdkmfyiq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhiwuduotai.top/gtvjupuxhl.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtlawmnnkd.html

Ruby: 42.to_s
来源：http://hz.ivvv.top/gtdrjjgfim.html

C#:   42.ToString()
来源：http://hz.shuidangran.top/gtykndcysm.html

[A08] 取整与四舍五入
来源：http://hz.nanxuanxn.top/gtckcbljsp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.zhoulong.xyz/gtrcqmkslx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.daria6918.cn/gtvtlxeriv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hammf.cn/gtsbiohetu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cheryme.top/gtzedqsmkv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yuxming.cn/gtqlwasrya.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.shangyingyoupin.top/gtjupeerma.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.nwbrower.top/gthytnfxmy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cqqwz.cn/gtvwlsqxql.html

[A09] 绝对值与最大最小值
来源：http://hz.316326.xyz/gtkuncrelb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gogol.net.cn/gteaggrffv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgfzy.top/gtnovlvwlc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xuetiantiany.cn/gtznswhglu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jianghu66.top/gtsimpjdjv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xuanzx.com/gtjkhtbsus.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhoulong.xyz/gtwevrlszq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ybcxt.top/gtuvolmajs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hammf.cn/gtriqpxmkh.html

[A10] 生成随机数
来源：http://hz.pengpengdd.cyou/gtuicuapvi.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sweek.top/gtqhqxchkm.html

PHP:  random_int(1, 100);
来源：http://hz.mhx1999.top/gtapgayskf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.kuanghao11.cn/gtgqqflldk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ywan-chungtsiang.top/gtwkkhkirk.html

Java: new Random().nextInt(100) + 1
来源：http://hz.chenjidiqi.icu/gtkwwwgruc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shuidangran.top/gtbnylynpq.html

Ruby: rand(1..100)
来源：http://hz.zhaomingkeji.xyz/gtnznagrpk.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinqigufen.top/gtpjxwzeib.html

[A11] 条件表达式（三元）
来源：http://hz.hfpthk.cn/gtbdfbfbyd.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.wangdashe.top/gtoiinoqxp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gttnxrxsym.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtydbbvuah.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigfzy.top/gtjbxqkced.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jyoumei.cn/gtukmakhez.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.cucudq.cn/gtrlptjmfd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.shangyingyoupin.top/gtonjppdcy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtrgmxzupc.html

[A12] 字符串插值 / 格式化
来源：http://hz.vqdsnc.cn/gtsusfwriz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.nwbrower.top/gtkqsxwwrx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.andypj.xyz/gtsbzblxum.html

JS:   `Hello, ${name}!`
来源：http://hz.mhx1999.top/gtdvgqakmk.html

TS:   `Hello, ${name}!`
来源：http://hz.yuxming.cn/gtvhqurgqr.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hammf.cn/gtvkwlvsgo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.iojbl.cn/gtkmqonecu.html

Ruby: "Hello, #{name}!"
来源：http://hz.haohaochexian.top/gtpdinelss.html

C#:   $"Hello, {name}!"
来源：http://hz.zhongyouzk.top/gtxbgogibf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yj20258888.top/gtxbyhtjtc.html

Py:   "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtimwquycs.html

PHP:  "第一行\n第二行"
来源：http://hz.sweek.top/gtozmmxxie.html

JS:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gtuiexftsa.html

TS:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtxtievmoz.html

Java: "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtsgiajggf.html

Go:   "第一行\n第二行"
来源：http://hz.0kj1m.cn/gttupvaxyf.html

Ruby: "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtingeslnm.html

C#:   "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtnwhnrkas.html

[A14] 注释写法
来源：http://hz.hywenlv.cn/gtkndaaxxz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ybcxt.top/gteklaombt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yj202588.top/gtgnzprszd.html

JS:   // 单行；/* 多行 */
来源：http://hz.hysaishi.cn/gtdntwstyj.html

TS:   // 单行；/* 多行 */
来源：http://hz.aizwys.cn/gtvovoxlyx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sufxvd.cn/gtxkjugsls.html

Go:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtaomkcqnv.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.snrcjt.cn/gtrptqxxjn.html


<!-- 参考信息 -->