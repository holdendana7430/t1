代发 wailian999

[U85] JS：可选链
来源：http://hz.andypj.xyz/gtgubtxvyq.html

a?.b?.c
来源：http://hz.c1oappe.top/gtyuxqusht.html

[U86] JS：空值合并
来源：http://hz.guowangkeji.top/gtbrsfigef.html

a ?? b
来源：http://hz.feifeiyinyue.top/gtwmefhntk.html

[U87] JS：解构默认值
来源：http://hz.sufxvd.cn/gtrzstjfba.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangdashe.top/gtzmkxhevf.html

[U88] JS：对象展开合并
来源：http://hz.yuanzhike.top/gtaytdpwob.html

{ ...a, ...b }
来源：http://hz.jyoumei.cn/gthxxmslqz.html

[U89] JS：数组去重
来源：http://hz.quarkkingdee.top/gtukjnljyu.html

[...new Set(arr)]
来源：http://hz.hammf.cn/gttahdkbnk.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtvlmetyra.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtktyuzycr.html

[U91] JS：对象键值遍历
来源：http://hz.mhx1999.top/gthswvwanu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258.top/gtnilnimtx.html

[U92] JS：深拷贝
来源：http://hz.nanxuanxn.top/gtrzbsdyyy.html

structuredClone(obj)
来源：http://hz.guowangkeji.top/gtzoszhahs.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtxsgfzbjm.html

`共 ${n} 条`
来源：http://hz.jyoumei.cn/gtmnmwxgbs.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtelrrbqwi.html

const double = x => x * 2;
来源：http://hz.cheryme.top/gtiyjhlzky.html

[U95] JS：Promise 包装
来源：http://hz.hongshengwenyu.top/gtlxxlpspj.html

new Promise((resolve, reject) => {})
来源：http://hz.hywenlv.cn/gtzoaoveeo.html

[U96] JS：async/await 与异常
来源：http://hz.hongshengwenyu.top/gtkgqwewfm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtmyknhinn.html

[U97] JS：并发请求
来源：http://hz.cucudq.cn/gtzvyonfgr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtwxctifya.html

[U98] JS：fetch 带 JSON
来源：http://hz.yanxiufei.cn/gtzpyffkvk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258.top/gtwhrztoxh.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtxwrtuzqy.html

el.addEventListener("click", e => {})
来源：http://hz.jinghuilouyu.cn/gtlbonzbwr.html

[U100] JS：DOM 查询
来源：http://hz.shanyushiyangkeji.top/gtsntvnhfj.html

document.querySelector(".item")
来源：http://hz.yvedp.cn/gtfxvppavv.html

[U101] JS：classList 操作
来源：http://hz.chenzaomai.com/gtsoyxlkik.html

el.classList.toggle("active")
来源：http://hz.hfpthk.cn/gtefzlaedo.html

[U102] JS：本地存储
来源：http://hz.hongshengwenyu.top/gtxomfdxla.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xinyue.icu/gtcycyudxk.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtrkbpqxjo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.fengsongda.top/gtcfuujnkz.html

[U104] JS：防抖
来源：http://hz.wangshuangyany.cn/gtqzcogxbp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gttfxhmjas.html

[U105] JS：节流
来源：http://hz.pengpengdd.cyou/gtehuxfeln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hywenlv.cn/gtyltnsags.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtnpkkdacy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.mhx1999.top/gtebninciy.html

[U107] JS：数字千分位
来源：http://hz.cucudq.cn/gtvucpdukf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydzc1.top/gtazgwtygq.html

[U108] JS：随机整数
来源：http://hz.tanke756.top/gteivzcaie.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hammf.cn/gtrwkwnhcg.html

[U109] JS：数组分组
来源：http://hz.yonumen.top/gtxktxnxmn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtoqcctovr.html

[U110] JS：数组分块
来源：http://hz.xylfe.cn/gtzbutouuy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jianghu66.top/gtabqvssyk.html

[U111] JS：对象转 Map
来源：http://hz.jinyuanbaomall.cn/gtejsrqjjo.html

new Map(Object.entries(obj))
来源：http://hz.ppjwa.cn/gtthhknkjx.html

[U112] JS：字符串补位
来源：http://hz.svipenyu.cn/gtvuvidauo.html

"7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtcyoyqukm.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gthsxdpekm.html

s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtfxncnaux.html

[U114] JS：JSON 深比较
来源：http://hz.yonumen.top/gtnbdtmsbe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtvjzquloc.html

[U115] JS：生成 UUID
来源：http://hz.xuetiantiany.cn/gtzwajzdmt.html

crypto.randomUUID()
来源：http://hz.dashuyun.cn/gthlxtshjw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtsaxjalwl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258.top/gtpfukwrne.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gtsewzoxzq.html

npm i -D vitest;  npx vitest
来源：http://hz.hywenlv.cn/gtfwahmdoq.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtecavdmbn.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gthjaosemr.html

[U119] JS：生产构建
来源：http://hz.zycfv.cn/gtppcsujtj.html

npx vite build
来源：http://hz.meibo888.top/gtlfvwyhvr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnxiangtu.top/gtvnawpwiu.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gtkwwwwgnn.html

================================================================================
来源：http://hz.aizwys.cn/gtxyqknmhy.html

统计汇总
来源：http://hz.iojbl.cn/gtvtipkzbh.html

================================================================================
来源：http://hz.52xcode.cn/gtbxgcggey.html

按语言统计（条）：
来源：http://hz.iojbl.cn/gtcoounwwc.html

Python ......... 252
来源：http://hz.gotoacloud.top/gtjbznfeke.html

PHP ............ 252
来源：http://hz.yj20258.top/gtmpeowtrg.html

JavaScript ..... 252
来源：http://hz.tanke756.top/gtrhhbvmyq.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gthrmdxhji.html

Java ........... 212
来源：http://hz.shangyingyoupin.top/gtzfhcojlq.html

Go ............. 212
来源：http://hz.xingfuxueyuan.xyz/gtmwuohldt.html

Ruby ........... 212
来源：http://hz.sysykeji.top/gtbuojddfl.html

C# ............. 212
来源：http://hz.chenlongwang.top/gtnkufphal.html

C .............. 30
来源：http://hz.yueranfly.top/gtqjmxmwgs.html

C++ ............ 30
来源：http://hz.pycfn.com/gtdpmcrbjr.html

SQL ............ 90
来源：http://hz.cdnleiting.top/gtilsmtntt.html

Bash ........... 80
来源：http://hz.hongshengwenyu.top/gtbcezoofi.html

Kotlin ......... 15
来源：http://hz.yj20258.top/gtmvzrvwvh.html

Swift .......... 15
来源：http://hz.vqdsnc.cn/gtobmjeuiv.html

Lua ............ 10
来源：http://hz.hongshengwenyu.top/gtplxrurhl.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtbjbbporz.html

Scala .......... 10
来源：http://hz.hywenlv.cn/gtdryjoegu.html

------------------------------------
来源：http://hz.nwbrower.top/gtzdoqbezc.html

合计 ........... 2106 条
来源：http://hz.sysykeji.top/gtorqdxtgt.html

按章节统计：
来源：http://hz.quarkkingdee.top/gtemkrfuuk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtwcjvobrl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtihizgyhn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtsmqgnckl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhixingplan.top/gthbtmlmqb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ppjwa.cn/gtrammwmds.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xinyue.icu/gtviqfijec.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gtfltffbfk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xuanzx.com/gthfarxasb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtcfubueln.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yvedp.cn/gtrjmzwsex.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtblpgjtne.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtapjidepj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtvsplqdtj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtagjecxzn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxuanxn.top/gtfzliaeow.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtulrzdxvo.html

Q SQL 专题                              90
来源：http://hz.yonumen.top/gtubpakgkf.html

R Bash 专题                             80
来源：http://hz.pengpengdd.cyou/gtcfeuhige.html

S C / C++ 专题                          60
来源：http://hz.vqdsnc.cn/gtvmgcpqqr.html

T 其他语言补充                          60
来源：http://hz.ehwqpu.com/gtbiujjnft.html

U 高频实用片段                         120
来源：http://hz.sxryk.cn/gtkosqsuhu.html

------------------------------------
来源：http://hz.cdnleiting.top/gtthsnmavo.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtuhnfjrgn.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtbauxkkdg.html

使用提醒
来源：http://hz.redwolf501.top/gtkreezqaj.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtanrrrqsn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.iojbl.cn/gtcbedjxhf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.52xcode.cn/gtyugyhbpk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.pengpengdd.cyou/gtlsaqotzc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.andypj.xyz/gtargzguws.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zdqjudy.top/gtjfqwgpbp.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gtpgrjoqyf.html

================================================================================
来源：http://hz.yangfankeji.com/gtpmlutnmy.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.daxiang520.top/gtodottzpp.html

Common Programming Examples Cheat Book
来源：http://hz.svipenyu.cn/gtykapumpp.html

================================================================================
来源：http://hz.zhengqikj.top/gtdjfmswte.html

【收录内容】
来源：http://hz.jyoumei.cn/gtywtkgksn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinyuanbaomall.cn/gtdwranfcz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shuidangran.top/gtgqlagljf.html

SQL · Bash · C · C++
来源：http://hz.jqgufenzy.top/gtwwmiuafn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtjfyxwjje.html

【使用说明】
来源：http://hz.cdnleiting.top/gtokdttspe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jiagoushi.top/gttksuiugw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ehwqpu.com/gtrgxnwzit.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xylfe.cn/gtoszfehgo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shzxlz.cn/gtdrltbqsi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nwbrower.top/gtyrpdmehm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ppjwa.cn/gtiqnmjyre.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgfzy.top/gtnyrexxse.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xingfuxueyuan.xyz/gtokcpyifw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.guowangkeji.top/gtvmyfhabx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinqigufen.top/gtgqscoihi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydjk.org.cn/gtckhhabwv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zycfv.cn/gtrylhcdyf.html

【文件统计】
来源：http://hz.0kj1m.cn/gtnubmncpv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shangyingyoupin.top/gtvwxjonxe.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtnvjbklhk.html

目  录
来源：http://hz.dashuyun.cn/gtrjdxwcbc.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gtgzfmpcbs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtxwnrfpwx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aibaodan.cn/gtpjawznrb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gteflpblqx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinqigfzy.top/gtbvolooik.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aizwys.cn/gtoabgttpl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gttneojcip.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtgzeeloou.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hfpthk.cn/gtwhfxmsol.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtqmywsdqd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtvgyttyno.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtegwztjgh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtsuepphlc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtyoowzgyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gtnifuzlkr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cucudq.cn/gtrbokipqt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gttyrxbtyx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.redwolf501.top/gtvukwnfrh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ivvv.top/gtsfwnetna.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shuidangran.top/gtyeyxktdk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtbgalwwhh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtqwjburpu.html

================================================================================
来源：http://hz.sufxvd.cn/gtnxhfgtia.html

A. 基础语法与类型
来源：http://hz.yonumen.top/gtqssfvcjd.html

================================================================================
来源：http://hz.zhengqikj.top/gtfylascqu.html

[A01] Hello World
来源：http://hz.bjfxy.top/gtbfbeuvwi.html

Py:   print("Hello, World!")
来源：http://hz.xuanzx.com/gtzqdmhuhc.html

PHP:  echo "Hello, World!";
来源：http://hz.xuetiantiany.cn/gtqvbdlqxs.html

JS:   console.log("Hello, World!");
来源：http://hz.hnxiangtu.top/gtubjaboyh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hammf.cn/gtnkwqgsae.html

Java: System.out.println("Hello, World!");
来源：http://hz.ybcxt.top/gtgymxvhfh.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydjk.org.cn/gtbqxiawxj.html

Ruby: puts "Hello, World!"
来源：http://hz.yuxming.cn/gtingzklvj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gthqoopyfj.html

[A02] 变量声明与赋值
来源：http://hz.hfpthk.cn/gtbwprbscp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cashguo.top/gtvjecbcib.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtkaqqvsnp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yangfankeji.com/gtughbsiaq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.daxiang520.top/gtvpnqcjxm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtxiejljof.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtmwurzpfx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cqqwz.cn/gtqvurrkje.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hywenlv.cn/gtmhxcoric.html

[A03] 常量定义
来源：http://hz.xuanzx.com/gtnzwigvin.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj202588.top/gtsuybrusp.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gttofpitvc.html

JS:   const PI = 3.14159;
来源：http://hz.ehwqpu.com/gtwxafvlin.html

TS:   const PI: number = 3.14159;
来源：http://hz.andypj.xyz/gtiteapxlv.html

Java: static final double PI = 3.14159;
来源：http://hz.cheryme.top/gtnkigeesa.html

Go:   const PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtbhsgjcsb.html

Ruby: PI = 3.14159
来源：http://hz.nanxinkj.top/gtvfkqlmir.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtuptlpbqq.html

[A04] 判断变量类型
来源：http://hz.gzhubu.top/gtcxdyxfjc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jianghu66.top/gtqjmeuoyq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dashuyun.cn/gtdxlzpsiy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhongyouzk.top/gtsiyeyxxe.html

TS:   typeof x; x instanceof Date
来源：http://hz.ywan-chungtsiang.top/gtulmsiskg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shuidangran.top/gtpveffift.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gtslfvmwbl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.pengpengdd.cyou/gtbjfddicv.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhongyouzk.top/gtedaoupsu.html

[A05] 整数除法与取模
来源：http://hz.zhoulong.xyz/gtrcbexxra.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yongpay.top/gtxwyffbuv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yvedp.cn/gtbjcnvlov.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zdqjudy.top/gtuyvabzwk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sxryk.cn/gthmfptqfe.html

Java: 7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gtpturblfw.html

Go:   7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtlwhfxpup.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtluaothxj.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuxming.cn/gtheylnpov.html

[A06] 字符串转数字
来源：http://hz.quarkkingdee.top/gtoiqblobv.html

Py:   int("42"); float("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtacpnwlcv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hywenlv.cn/gtvtkbpywg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xylfe.cn/gtzwimuwee.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.nwbrower.top/gtlswmxhns.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhixingplan.top/gtredztdas.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shanyushiyangtech.top/gtdsasomxc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.tanke756.top/gtrinzxdha.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.quarkkingdee.top/gtetumpbkh.html

[A07] 数字转字符串
来源：http://hz.tianlin.xyz/gtsyllhudj.html

Py:   str(42)
来源：http://hz.bjfxy.top/gthaxhczbv.html

PHP:  (string) 42; strval(42)
来源：http://hz.0kj1m.cn/gtdrvmlrft.html

JS:   String(42); (42).toString()
来源：http://hz.hfpthk.cn/gtbwvwbpgy.html

TS:   String(42)
来源：http://hz.guannengcc.top/gttgzzniyf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yj20258888.top/gtljskirqo.html

Go:   strconv.Itoa(42)
来源：http://hz.snrcjt.cn/gtswfjmbwn.html

Ruby: 42.to_s
来源：http://hz.yuanzhike.top/gtyfudgwde.html

C#:   42.ToString()
来源：http://hz.pengpengdd.cyou/gtfezcaafv.html

[A08] 取整与四舍五入
来源：http://hz.shuidangran.top/gtigheyolv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yangfankeji.com/gthnaqynff.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xuanzx.com/gthgdjayup.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gaohongyu789.top/gtzfhywayb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.dianchejie.cn/gtmpbehoev.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhixingplan.top/gtkmkkdgoq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.316326.xyz/gtyeabcina.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.pycfn.com/gtussqbdzv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ehwqpu.com/gtkyrdoxdj.html

[A09] 绝对值与最大最小值
来源：http://hz.jinghuilouyu.cn/gtrdcwdcle.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.daxiang520.top/gtdeaxsfbe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtzdcuvxsf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jqgfzy.top/gtwfkjbqjo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigufen.top/gtknjxjyib.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.cucudq.cn/gtqezqrejz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.meibo888.top/gtylnwrahs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cdnleiting.top/gtflqurqtw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zycfv.cn/gtikjofgtb.html

[A10] 生成随机数
来源：http://hz.shangyingyoupin.top/gtfoprucfy.html

Py:   import random; random.randint(1, 100)
来源：http://hz.meibo888.top/gtljjrfmnq.html

PHP:  random_int(1, 100);
来源：http://hz.yueranfly.top/gtbjjbvedl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yanxiufei.cn/gtffbqyhjn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jyoumei.cn/gtaqvjvjwf.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cucudq.cn/gtjuygkhqn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhixingplan.top/gtkqjwhvzy.html

Ruby: rand(1..100)
来源：http://hz.shuidangran.top/gttjldezqg.html

C#:   new Random().Next(1, 101)
来源：http://hz.hywenlv.cn/gtjfptwhpi.html

[A11] 条件表达式（三元）
来源：http://hz.meibo888.top/gtgayodemi.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shanyushiyangkeji.top/gtfagvkbmm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtnnezaklq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gtskghnkvz.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gttermigsy.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtqtciygao.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jinqigfzy.top/gtzbznbqhk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtwjiqibso.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.dianchejie.cn/gtotupgvhy.html

[A12] 字符串插值 / 格式化
来源：http://hz.ybcxt.top/gtqduhsadn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.cucudq.cn/gtqvdpewvb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jyoumei.cn/gttiejtiuw.html

JS:   `Hello, ${name}!`
来源：http://hz.jiagoushi.top/gtqtuyeiky.html

TS:   `Hello, ${name}!`
来源：http://hz.ppjwa.cn/gtzvyeaewo.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.tanke756.top/gtypybokar.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.cdnleiting.top/gtwfvqktvk.html

Ruby: "Hello, #{name}!"
来源：http://hz.hammf.cn/gtjubnbksb.html

C#:   $"Hello, {name}!"
来源：http://hz.quarkkingdee.top/gtrcfkprrm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.9152youxi.cn/gtkdmxqojx.html

Py:   "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtofeuddzp.html

PHP:  "第一行\n第二行"
来源：http://hz.svipenyu.cn/gtybsfqrrq.html

JS:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtvneabwxv.html

TS:   "第一行\n第二行"
来源：http://hz.jianghu66.top/gtuiekyztr.html

Java: "第一行\n第二行"
来源：http://hz.52xcode.cn/gthzrvnqmz.html

Go:   "第一行\n第二行"
来源：http://hz.hammf.cn/gtulgwzwxc.html

Ruby: "第一行\n第二行"
来源：http://hz.shanyushiyangkeji.top/gtzehlopha.html

C#:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtogcpvvwx.html

[A14] 注释写法
来源：http://hz.hfpthk.cn/gtogrhwndq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jiagoushi.top/gtkiozovir.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ppjwa.cn/gtmzsuxkvi.html

JS:   // 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtvlrieqln.html


<!-- 参考信息 -->