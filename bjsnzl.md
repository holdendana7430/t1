代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.ywan-chungtsiang.top/gtjkuontxg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhijiandao.cn/gtshhdcrbi.html

[U92] JS：深拷贝
来源：http://hz.fengsongda.top/gtvpckysum.html

structuredClone(obj)
来源：http://hz.dashuyun.cn/gtbrvjalri.html

[U93] JS：模板字符串
来源：http://hz.daria6918.cn/gtrnqoguyh.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtunvzyfpi.html

[U94] JS：箭头函数
来源：http://hz.hongshengwenyu.top/gttcifqxed.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtvbchyxzr.html

[U95] JS：Promise 包装
来源：http://hz.zycfv.cn/gtrmuytztm.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gtefmxmstw.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gtljomfjwx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtqcrndgvv.html

[U97] JS：并发请求
来源：http://hz.sysykeji.top/gtbpreowvf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtmvuamwyr.html

[U98] JS：fetch 带 JSON
来源：http://hz.yuanzhike.top/gtugxjjgni.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinyuanbaomall.cn/gtxcgvjpha.html

[U99] JS：事件监听
来源：http://hz.havefunace.top/gtilrazvyd.html

el.addEventListener("click", e => {})
来源：http://hz.nwbrower.top/gtgaykdigl.html

[U100] JS：DOM 查询
来源：http://hz.hfpthk.cn/gtavqqkdhp.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtaywhdcwl.html

[U101] JS：classList 操作
来源：http://hz.xuanzx.com/gtjzcfdfin.html

el.classList.toggle("active")
来源：http://hz.316326.xyz/gtomitmzfq.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gteofrlwfn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.snrcjt.cn/gtetjzmeqg.html

[U103] JS：定时器
来源：http://hz.ppjwa.cn/gtjcczcfba.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtzxdfvbdo.html

[U104] JS：防抖
来源：http://hz.shanyushiyangkeji.top/gthiyuqtgx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtpvstigzq.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtewdtuzmh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.guannengcc.top/gtzrvlbxel.html

[U106] JS：日期格式化
来源：http://hz.ehwqpu.com/gtlyflvphu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cashguo.top/gthutvllle.html

[U107] JS：数字千分位
来源：http://hz.sweek.top/gtdwinendm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hfpthk.cn/gtynjwwdto.html

[U108] JS：随机整数
来源：http://hz.daria6918.cn/gtotsexznu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydjk.org.cn/gtoebumwxh.html

[U109] JS：数组分组
来源：http://hz.hnqzz.top/gtrzluenxi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gthkajhore.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtisvtonac.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gtiiwqbpxs.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gtawmmywyt.html

new Map(Object.entries(obj))
来源：http://hz.xylfe.cn/gtztuuruan.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gtenjmhvbx.html

"7".padStart(3, "0")
来源：http://hz.pycfn.com/gtymqiureg.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gtwiviczfz.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtgaaseiyg.html

[U114] JS：JSON 深比较
来源：http://hz.mhx1999.top/gtkhvxmvvc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gtblfuxjgi.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtonjfzbuk.html

crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtnfwzqbuo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.kuanghao11.cn/gtawlbkelv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.vqdsnc.cn/gtkblkbigz.html

[U117] JS：单元测试
来源：http://hz.hnqzz.top/gtsrgjmhkf.html

npm i -D vitest;  npx vitest
来源：http://hz.pengpengdd.cyou/gthqpsefjh.html

[U118] JS：开发服务器
来源：http://hz.dashuyun.cn/gtevurclzb.html

npm i -D vite;  npx vite
来源：http://hz.wangshuangyany.cn/gtffegdlij.html

[U119] JS：生产构建
来源：http://hz.tianlin.xyz/gtrkhrpvrj.html

npx vite build
来源：http://hz.hysaishi.cn/gtsvgsuhio.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtxzzcfgfr.html

import.meta.env.VITE_API_URL
来源：http://hz.gzhubu.top/gtqwqksobu.html

================================================================================
来源：http://hz.c1oappe.top/gtjwcpylst.html

统计汇总
来源：http://hz.shuidangran.top/gtkjtuqyiy.html

================================================================================
来源：http://hz.hfpthk.cn/gtesvjlboy.html

按语言统计（条）：
来源：http://hz.daria6918.cn/gtvvjdyswz.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtxpblmwbx.html

PHP ............ 252
来源：http://hz.yvedp.cn/gtyezeugda.html

JavaScript ..... 252
来源：http://hz.ivvv.top/gtgkzhoxus.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtapupvezu.html

Java ........... 212
来源：http://hz.fzhhl.top/gtxzirdgoo.html

Go ............. 212
来源：http://hz.mhx1999.top/gtyvfkahjm.html

Ruby ........... 212
来源：http://hz.yj202588.top/gtkrqovwnv.html

C# ............. 212
来源：http://hz.cheryme.top/gtlvatgnca.html

C .............. 30
来源：http://hz.aizwys.cn/gtqgqjcsje.html

C++ ............ 30
来源：http://hz.havefunace.top/gtarkyjepj.html

SQL ............ 90
来源：http://hz.aizwys.cn/gteeyvupvq.html

Bash ........... 80
来源：http://hz.jianghu66.top/gtskofnehe.html

Kotlin ......... 15
来源：http://hz.shuidangran.top/gtlusujirh.html

Swift .......... 15
来源：http://hz.meibo888.top/gthmyytpfu.html

Lua ............ 10
来源：http://hz.hfpthk.cn/gtvpujjlgv.html

Perl ........... 10
来源：http://hz.zhijiandao.cn/gtwttbmpol.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtlgprugom.html

------------------------------------
来源：http://hz.jianghu66.top/gtjqltoryl.html

合计 ........... 2106 条
来源：http://hz.ppjwa.cn/gtapmxwnoz.html

按章节统计：
来源：http://hz.xziqi.cn/gtigkborrk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.andypj.xyz/gtmflrekus.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtcvliipsp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yonumen.top/gtabslxecv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cdnleiting.top/gtmxznncbj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydjk.org.cn/gtumijhhfv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtmsauwlfq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtqkbbmdka.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gttdprybgu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtpossumrn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.vqdsnc.cn/gtxxgjmuls.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtukxhebbf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtwujoijvu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtjqfpneym.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtzjzudowd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gthlorsvnj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtytfufonk.html

Q SQL 专题                              90
来源：http://hz.ybcxt.top/gtkjehfwln.html

R Bash 专题                             80
来源：http://hz.zhoulong.xyz/gtzchiukez.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtjpnklksc.html

T 其他语言补充                          60
来源：http://hz.wangdashe.top/gtyyyhubpq.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gttpmopfjt.html

------------------------------------
来源：http://hz.zycfv.cn/gtvvbwvkft.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtbnzaneei.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtldxpqzpx.html

使用提醒
来源：http://hz.cucudq.cn/gtmillktyt.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtcfwvtivu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cucudq.cn/gtesuzfoyo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuxming.cn/gtzgyidsij.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sweek.top/gtwvbjxkej.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yonumen.top/gtlvdaqwsa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sufxvd.cn/gtmcrabxcn.html

—— 文件结束 ——
来源：http://hz.yj20258.top/gtqzgepdvi.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdtoupcep.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtkljdwdhm.html

Common Programming Examples Cheat Book
来源：http://hz.yueranfly.top/gtkjtfrodv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtufcvuohj.html

【收录内容】
来源：http://hz.yueranfly.top/gtagyraqwz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sysykeji.top/gttsnroutb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jqgufenzy.top/gttedxskzl.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gtiqcmjnbn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.9152youxi.cn/gtisgblezb.html

【使用说明】
来源：http://hz.yonumen.top/gtpdrrbbkq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gaohongyu789.top/gtngmkjcmj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydzc1.top/gtwrdxryuc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sysykeji.top/gtiiysmkdl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ybcxt.top/gtsprqoobb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhongyouzk.top/gttybcnikk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhaomingkeji.xyz/gttdfnskem.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhixingplan.top/gtzojvocar.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hnqzz.top/gtqmbgayfk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shzxlz.cn/gtxqsmbxqs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinghuilouyu.cn/gtdsuthsqb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.snrcjt.cn/gtjyagdavg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aibaodan.cn/gtupladxcv.html

【文件统计】
来源：http://hz.yonumen.top/gtfwnkejvw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.aibaodan.cn/gtqrabokzk.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtxhdynzgr.html

目  录
来源：http://hz.nwbrower.top/gtzwaoarlj.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtqyeeeauw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.fzhhl.top/gtzmhbxkok.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtojnogixg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jiagoushi.top/gtmquvdbdb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtryovxshh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ppjwa.cn/gtubwtwkau.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.birdmap.top/gtkpogvspm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtdpwglfxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sysykeji.top/gtlcdevqkx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gteckgxxyr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinyuanbaomall.cn/gtsorwsuqm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtytgkzqko.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtsqlqknqf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gteitcuvvq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gtbtyumaar.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.daria6918.cn/gtiapxkyxv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtpfibvfzd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.aibaodan.cn/gtpiiqctqa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenzaomai.com/gtwuxlkzkw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gzhubu.top/gtqybtgouc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gtewwkxwom.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gtakvzmtkt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzetkwkrg.html

A. 基础语法与类型
来源：http://hz.quarkkingdee.top/gtabzgscfs.html

================================================================================
来源：http://hz.ppjwa.cn/gtzxiykihz.html

[A01] Hello World
来源：http://hz.hammf.cn/gtadxuwfxq.html

Py:   print("Hello, World!")
来源：http://hz.gzhubu.top/gtsnrnlfki.html

PHP:  echo "Hello, World!";
来源：http://hz.hnxiangtu.top/gtkwhpiixc.html

JS:   console.log("Hello, World!");
来源：http://hz.guowangkeji.top/gtxuttvnbs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wangshuangyany.cn/gtwtmpfuun.html

Java: System.out.println("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtsefwiqgs.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtaykrsizi.html

Ruby: puts "Hello, World!"
来源：http://hz.316326.xyz/gttxheykck.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.0kj1m.cn/gtaqxbwjqi.html

[A02] 变量声明与赋值
来源：http://hz.jinghuilouyu.cn/gtoifncrnf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.daxiang520.top/gtecdomnrl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.snrcjt.cn/gtrngilcsk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ehwqpu.com/gtqvfilndo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.nanxinkj.top/gtufwejvmd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtlxdfqkop.html

Go:   name := "Alex"; age := 20
来源：http://hz.nwbrower.top/gthjjdxyjl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhixingplan.top/gteazeykup.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtcnppjxdx.html

[A03] 常量定义
来源：http://hz.shuidangran.top/gttamiouim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sufxvd.cn/gtjjcnkusp.html

PHP:  const PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtckjdanaf.html

JS:   const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtwbgljoiq.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtcrugadrw.html

Java: static final double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtgvxinmnp.html

Go:   const PI = 3.14159
来源：http://hz.shangyingyoupin.top/gtitswhggp.html

Ruby: PI = 3.14159
来源：http://hz.shuidangran.top/gtnhlmbzox.html

C#:   const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtakrzqger.html

[A04] 判断变量类型
来源：http://hz.andypj.xyz/gtrsxxdiqy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydjk.org.cn/gtdnfwwgeo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.svipenyu.cn/gtveonobgo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.haohaochexian.top/gtqnytoorj.html

TS:   typeof x; x instanceof Date
来源：http://hz.hfpthk.cn/gtoqterkgg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.9152youxi.cn/gtjqpcspvp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yueranfly.top/gtoadwwhfk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhiwuduotai.top/gtgsbcekre.html

C#:   x.GetType().Name; x is int
来源：http://hz.fengsongda.top/gtcrqdqgjy.html

[A05] 整数除法与取模
来源：http://hz.zdqjudy.top/gtqlwnhdbc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yueranfly.top/gtrtsuagnw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.andypj.xyz/gtfjferyia.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuetiantiany.cn/gtblmdrckt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xziqi.cn/gtbevhxrmq.html

Java: 7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtqdanvrsn.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtdqyfhnxo.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtvfrxfxvf.html

C#:   7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtrieprfaj.html

[A06] 字符串转数字
来源：http://hz.zhaomingkeji.xyz/gtebhjywmn.html

Py:   int("42"); float("3.14")
来源：http://hz.fengsongda.top/gthpjjjbsp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.sufxvd.cn/gtgwxeeirl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhiwuduotai.top/gtowtoucgd.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cqqwz.cn/gtqjwrqolq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.andypj.xyz/gthxuweoll.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hfpthk.cn/gtkjefipve.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.chenjidiqi.icu/gtowawxdbl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.iojbl.cn/gtjaskxyiz.html

[A07] 数字转字符串
来源：http://hz.chenzaomai.com/gtuqijwnhc.html

Py:   str(42)
来源：http://hz.pycfn.com/gthsbqdfnh.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhoulong.xyz/gtxglabuxc.html

JS:   String(42); (42).toString()
来源：http://hz.svipenyu.cn/gtbxlqwoow.html

TS:   String(42)
来源：http://hz.chenjidiqi.icu/gtxpsylfvr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.vqdsnc.cn/gtwlmzsdgj.html

Go:   strconv.Itoa(42)
来源：http://hz.nwbrower.top/gtgculvkcz.html

Ruby: 42.to_s
来源：http://hz.nanxuanxn.top/gtbxswyqpm.html

C#:   42.ToString()
来源：http://hz.mhx1999.top/gtbgrrjtdt.html

[A08] 取整与四舍五入
来源：http://hz.snrcjt.cn/gtekgytqwu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yuxming.cn/gtrmelmvlw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hnxiangtu.top/gtvnzbskzc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gogol.net.cn/gtcgvgufox.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangtech.top/gtkomqzcyb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtsqpwadij.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.redwolf501.top/gtvivntlds.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.pycfn.com/gtikybvbkb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sweek.top/gttugxstck.html

[A09] 绝对值与最大最小值
来源：http://hz.shangyingyoupin.top/gtxjzssves.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuxming.cn/gtflgzwkmy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cucudq.cn/gtmihsvqlg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nwbrower.top/gtcuyftwwo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxuanxn.top/gtpmtkjedz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtdsofgxxk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj20258.top/gtrulytbxx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.havefunace.top/gtjlyhuyar.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jyoumei.cn/gtkmmivetc.html

[A10] 生成随机数
来源：http://hz.redwolf501.top/gtltnvzeji.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xinyue.icu/gtzjlbdqzn.html

PHP:  random_int(1, 100);
来源：http://hz.zhoulong.xyz/gtjgoxocbw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sysykeji.top/gthvixezqy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj20258.top/gtamsjlvhg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yongpay.top/gtfvmclpxs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinqigufen.top/gtcydwipln.html

Ruby: rand(1..100)
来源：http://hz.shangyingyoupin.top/gtfxyquuyz.html

C#:   new Random().Next(1, 101)
来源：http://hz.aizwys.cn/gtssvdlrcz.html

[A11] 条件表达式（三元）
来源：http://hz.yuanzhike.top/gtavbybaaa.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shuidangran.top/gtysufhmmt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.fzhhl.top/gtahnrmkff.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtmdieunwi.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhixingplan.top/gtijlrxadg.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtwapaowyp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jinyuanbaomall.cn/gttsiuwfuj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.tanke756.top/gtgmbtxzug.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtoimpozel.html

[A12] 字符串插值 / 格式化
来源：http://hz.ywan-chungtsiang.top/gtssoulhqi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.birdmap.top/gtdkgcurzh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jlsjyb.cn/gtimbykgqc.html

JS:   `Hello, ${name}!`
来源：http://hz.jlsjyb.cn/gtmvskywnd.html

TS:   `Hello, ${name}!`
来源：http://hz.shzxlz.cn/gtlzmxpbsq.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jyoumei.cn/gtbdsaoptf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.ywan-chungtsiang.top/gtardwgeix.html

Ruby: "Hello, #{name}!"
来源：http://hz.hnqzz.top/gtbqesubfz.html

C#:   $"Hello, {name}!"
来源：http://hz.meibo888.top/gttyllkmlu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yj202588.top/gtilzjrgds.html

Py:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtnyrevvfa.html

PHP:  "第一行\n第二行"
来源：http://hz.yj20258888.top/gtzkhrirjz.html

JS:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtgswpcupx.html

TS:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtwfirjbor.html

Java: "第一行\n第二行"
来源：http://hz.ivvv.top/gtbxiymoxd.html

Go:   "第一行\n第二行"
来源：http://hz.aibaodan.cn/gtyuwwrldr.html

Ruby: "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtlvykzeqd.html

C#:   "第一行\n第二行"
来源：http://hz.andypj.xyz/gthpobfdxx.html

[A14] 注释写法
来源：http://hz.iojbl.cn/gtocnjnhap.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jinghuilouyu.cn/gtokhijnno.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zdqjudy.top/gtrmyzxgdi.html

JS:   // 单行；/* 多行 */
来源：http://hz.gzhubu.top/gtxhostsye.html

TS:   // 单行；/* 多行 */
来源：http://hz.yongpay.top/gtyqfbcflm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.smart0.xyz/gtwbrscbdk.html

Go:   // 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtltkcfbgj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.fengsongda.top/gtzirxyepq.html

C#:   // 单行；/* 多行 */
来源：http://hz.wangdashe.top/gtkxwwiayo.html

[A15] 空值判断与默认值
来源：http://hz.birdmap.top/gtfkdkcitc.html

Py:   value = data or "默认值"
来源：http://hz.pycfn.com/gtcjlufjrq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.dianchejie.cn/gtjyvakyci.html

JS:   const value = data ?? "默认值";
来源：http://hz.cqqwz.cn/gtavoyesoi.html

TS:   const value = data ?? "默认值";
来源：http://hz.daxiang520.top/gtavvcolyz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nanxinkj.top/gtgbmcistj.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hongshengwenyu.top/gtbazyuymn.html


<!-- 参考信息 -->