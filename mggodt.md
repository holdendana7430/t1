代发 wailian999

[U85] JS：可选链
来源：http://hz.cashguo.top/gtrylvfwzd.html

a?.b?.c
来源：http://hz.yanxiufei.cn/gthbteivjs.html

[U86] JS：空值合并
来源：http://hz.316326.xyz/gtrktgovue.html

a ?? b
来源：http://hz.yvedp.cn/gtdgzohvke.html

[U87] JS：解构默认值
来源：http://hz.cqqwz.cn/gttzsktkej.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtimyesxnb.html

[U88] JS：对象展开合并
来源：http://hz.chenjidiqi.icu/gthipyeura.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gthgarydva.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gtbhnncwba.html

[...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtguizcazb.html

[U90] JS：数字数组排序
来源：http://hz.cqqwz.cn/gtdmsnxmgv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtomtjsdjz.html

[U91] JS：对象键值遍历
来源：http://hz.yj202588.top/gteabmxbpc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zycfv.cn/gtbthtxjkp.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtafymrdtb.html

structuredClone(obj)
来源：http://hz.gogol.net.cn/gtynlzgjgl.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gteidocxrx.html

`共 ${n} 条`
来源：http://hz.fzhhl.top/gtshxsjoit.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gttpyxjxlh.html

const double = x => x * 2;
来源：http://hz.guowangkeji.top/gtiovvqmwl.html

[U95] JS：Promise 包装
来源：http://hz.jyoumei.cn/gtfdszkofc.html

new Promise((resolve, reject) => {})
来源：http://hz.316326.xyz/gtvsnhytwc.html

[U96] JS：async/await 与异常
来源：http://hz.c1oappe.top/gtsabrgfeb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtqjxfpgut.html

[U97] JS：并发请求
来源：http://hz.zhiwuduotai.top/gtysijmbgb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtbpbymmry.html

[U98] JS：fetch 带 JSON
来源：http://hz.sxryk.cn/gtxerytoiq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtnffxacss.html

[U99] JS：事件监听
来源：http://hz.zhoulong.xyz/gtysyxiphg.html

el.addEventListener("click", e => {})
来源：http://hz.redwolf501.top/gtetynrdfg.html

[U100] JS：DOM 查询
来源：http://hz.jinqigfzy.top/gtejrukkdp.html

document.querySelector(".item")
来源：http://hz.ydzc1.top/gtxkrimrds.html

[U101] JS：classList 操作
来源：http://hz.zhoulong.xyz/gtxqoqzlbt.html

el.classList.toggle("active")
来源：http://hz.52xcode.cn/gteltdeqkk.html

[U102] JS：本地存储
来源：http://hz.iojbl.cn/gtdaznzotk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.birdmap.top/gtcingyron.html

[U103] JS：定时器
来源：http://hz.daria6918.cn/gtrusxmpdu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cdnleiting.top/gteujnicks.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtluifmvsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtqvwxlifv.html

[U105] JS：节流
来源：http://hz.yj202588.top/gtovrsetsm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yueranfly.top/gtrhberigy.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtflarfjud.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gotoacloud.top/gtznlmibeo.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtddpazwlm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jlsjyb.cn/gtnezmuvgn.html

[U108] JS：随机整数
来源：http://hz.jqgfzy.top/gtblutdkgp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gtqfqcnwyg.html

[U109] JS：数组分组
来源：http://hz.shanyushiyangkeji.top/gtresanmsy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtuppihgak.html

[U110] JS：数组分块
来源：http://hz.wangdashe.top/gtwrjhsrdp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nanxuanxn.top/gttpbyyvwg.html

[U111] JS：对象转 Map
来源：http://hz.haohaochexian.top/gtkfwrevbj.html

new Map(Object.entries(obj))
来源：http://hz.hywenlv.cn/gtzvoyxoqu.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gttliocdvv.html

"7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gthgsponht.html

[U113] JS：正则替换全部
来源：http://hz.iojbl.cn/gtioecljhj.html

s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtgggxnedi.html

[U114] JS：JSON 深比较
来源：http://hz.aibaodan.cn/gtojzksbst.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtmoierdvi.html

[U115] JS：生成 UUID
来源：http://hz.jyoumei.cn/gtwaqaoofs.html

crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtbbbearhu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jyoumei.cn/gtkeixnluf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgufenzy.top/gtihwnjwha.html

[U117] JS：单元测试
来源：http://hz.nanxinkj.top/gtxlgluhit.html

npm i -D vitest;  npx vitest
来源：http://hz.chenjidiqi.icu/gtuzhaxeig.html

[U118] JS：开发服务器
来源：http://hz.shzxlz.cn/gtyjmikiwy.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtxropabpg.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtuiqzbgcl.html

npx vite build
来源：http://hz.yj20258.top/gttnrdmpha.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hfpthk.cn/gtliryadpu.html

import.meta.env.VITE_API_URL
来源：http://hz.xuetiantiany.cn/gtafsbvlfi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtvffujogr.html

统计汇总
来源：http://hz.shzxlz.cn/gthiptbnpu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdluqjmko.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtjubtcqii.html

Python ......... 252
来源：http://hz.chenjidiqi.icu/gtgzlgtizh.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtlxjphqns.html

JavaScript ..... 252
来源：http://hz.snrcjt.cn/gtzmrobwjb.html

TypeScript ..... 212
来源：http://hz.hysaishi.cn/gtowdesnvd.html

Java ........... 212
来源：http://hz.yueranfly.top/gtaetkzlgv.html

Go ............. 212
来源：http://hz.feifeiyinyue.top/gtoiuictdn.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtuqnattqh.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gtcjbzhmkb.html

C .............. 30
来源：http://hz.daxiang520.top/gtjqlaswot.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtkkupjxsy.html

SQL ............ 90
来源：http://hz.zhoulong.xyz/gtedkavyat.html

Bash ........... 80
来源：http://hz.bjfxy.top/gtkxrlllbv.html

Kotlin ......... 15
来源：http://hz.zhiwuduotai.top/gtusyjgxrw.html

Swift .......... 15
来源：http://hz.wangdashe.top/gteyhfjzoa.html

Lua ............ 10
来源：http://hz.feifeiyinyue.top/gtvvqwlyjf.html

Perl ........... 10
来源：http://hz.snrcjt.cn/gtddjrmuff.html

Scala .......... 10
来源：http://hz.nanxuanxn.top/gtncccpmtb.html

------------------------------------
来源：http://hz.jlsjyb.cn/gtwxrkbefu.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gtkdgdudbt.html

按章节统计：
来源：http://hz.mhx1999.top/gtpmwjxqvc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtpfqlffxj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gttsdzsvux.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtrfftnnqs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtkoywfzgk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hysaishi.cn/gtofxjlncz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtidckcxsf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtfndeutko.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtwwmtlbql.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtqbyvueth.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhongyouzk.top/gtyydxpamw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtcgiykhxt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtrpbnnlum.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtowdfjuym.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtrvthzrzv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtpfulfylg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtefstlheq.html

Q SQL 专题                              90
来源：http://hz.fzhhl.top/gtakzvkvvg.html

R Bash 专题                             80
来源：http://hz.nwbrower.top/gtithsfpda.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangtech.top/gtdjsuivcc.html

T 其他语言补充                          60
来源：http://hz.vqdsnc.cn/gtrxbzkwdr.html

U 高频实用片段                         120
来源：http://hz.xingfuxueyuan.xyz/gtajhegsyu.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtpfgsbgdo.html

合计                                  2106 条
来源：http://hz.zycfv.cn/gtyskogeno.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtxdeqyxry.html

使用提醒
来源：http://hz.zhengqikj.top/gtfyfntjir.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtlwtwmfno.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hnqzz.top/gtnxkhoahk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuxming.cn/gtxntodtsi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ybcxt.top/gtstrfxpcg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.smart0.xyz/gtzyvvmiti.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.kuanghao11.cn/gtzszalnwg.html

—— 文件结束 ——
来源：http://hz.hfpthk.cn/gtukztkczg.html

================================================================================
来源：http://hz.gzhubu.top/gtgmvbajcn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258.top/gtkkyqpkqi.html

Common Programming Examples Cheat Book
来源：http://hz.chenzaomai.com/gtinekrihy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwxhmhovk.html

【收录内容】
来源：http://hz.9152youxi.cn/gtkhyhfpwj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.wangdashe.top/gtjxbnagoj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.mhx1999.top/gtmhspjiuh.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gtvujqxddo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xziqi.cn/gtjawjgtpd.html

【使用说明】
来源：http://hz.yuxming.cn/gtqljecerr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hysaishi.cn/gtgjogdbby.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daria6918.cn/gtklzonvff.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hywenlv.cn/gtkfqfhjph.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yvedp.cn/gtwbwhicrr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtvsplqmnk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydjk.org.cn/gttncafkwf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.havefunace.top/gtbzccdnmm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhengqikj.top/gtfbviomob.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenzaomai.com/gtpswuinxr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xylfe.cn/gtcfenrakg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhongyouzk.top/gtfanfzwaq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shangyingyoupin.top/gtsezgfxzb.html

【文件统计】
来源：http://hz.nanxinkj.top/gtajmhkcus.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.meibo888.top/gthwcrmzhu.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtxozdsqez.html

目  录
来源：http://hz.xuanzx.com/gttrzftfcb.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtfsbuyvcz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gthbggkhxl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtswphkeui.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtyjfdhmly.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gtfaaqdvbx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ywan-chungtsiang.top/gtkipohwdk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtjaifaxfz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gtauiuljyr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ppjwa.cn/gtehxpavul.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtzojrzfis.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydzc1.top/gtahxdakds.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtpbbiyqjt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtjrenpbzb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtnzbcnuub.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtrrcofana.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yangfankeji.com/gtfsdavvgy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtnjpgnfac.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuetiantiany.cn/gtbjjhgtbe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.c1oappe.top/gtpevmesco.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zycfv.cn/gtxthudgce.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhijiandao.cn/gtsguweojd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cheryme.top/gtfbpbefom.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrkiwkqvi.html

A. 基础语法与类型
来源：http://hz.dianchejie.cn/gtfdkyevvv.html

================================================================================
来源：http://hz.havefunace.top/gtryfvtbkr.html

[A01] Hello World
来源：http://hz.52xcode.cn/gtauljrdrh.html

Py:   print("Hello, World!")
来源：http://hz.ivvv.top/gtpkehtizz.html

PHP:  echo "Hello, World!";
来源：http://hz.xuetiantiany.cn/gtyfvdekcz.html

JS:   console.log("Hello, World!");
来源：http://hz.xinyue.icu/gtlmefnrjo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258888.top/gtktomgede.html

Java: System.out.println("Hello, World!");
来源：http://hz.yvedp.cn/gtpngjdzdo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ivvv.top/gtndbsjoyq.html

Ruby: puts "Hello, World!"
来源：http://hz.cqqwz.cn/gtbrhsngbq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cheryme.top/gtrszpkasi.html

[A02] 变量声明与赋值
来源：http://hz.jinyuanbaomall.cn/gtxbqfitdt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.kuanghao11.cn/gthjiddhuu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtfiuczrcj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.52xcode.cn/gtkeodwqvs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj202588.top/gtsnfjjlsm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sysykeji.top/gtbqennwfy.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgfzy.top/gtbahyliht.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj202588.top/gtvuqvkyft.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtcpwzarqj.html

[A03] 常量定义
来源：http://hz.jinghuilouyu.cn/gtytyvanay.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj202588.top/gtnxcjsgyt.html

PHP:  const PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtggakhjel.html

JS:   const PI = 3.14159;
来源：http://hz.yj20258888.top/gtxxpjuqcd.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtpqngjszp.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gteimyzfsu.html

Go:   const PI = 3.14159
来源：http://hz.yangfankeji.com/gtxvkvrwel.html

Ruby: PI = 3.14159
来源：http://hz.hnxiangtu.top/gtfrxgfprv.html

C#:   const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtqtctfwji.html

[A04] 判断变量类型
来源：http://hz.hfpthk.cn/gtuovqzapv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aibaodan.cn/gtojwmuahc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hammf.cn/gtiqqunkid.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.316326.xyz/gtbfffottc.html

TS:   typeof x; x instanceof Date
来源：http://hz.cdnleiting.top/gteubahkld.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ybcxt.top/gtgduilitv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.0kj1m.cn/gtnkrrhjnh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.9152youxi.cn/gtwcemzgex.html

C#:   x.GetType().Name; x is int
来源：http://hz.daxiang520.top/gtydyqzenk.html

[A05] 整数除法与取模
来源：http://hz.zycfv.cn/gtwszyuwab.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tian-w.cn/gtyloubmwt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtsgdmvdpp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtyilcneec.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtveoxbrkm.html

Java: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtkmvnawwe.html

Go:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtvrjgxysq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtosuelyme.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangdashe.top/gtxdtuyjsu.html

[A06] 字符串转数字
来源：http://hz.aizwys.cn/gtkhfeijgj.html

Py:   int("42"); float("3.14")
来源：http://hz.shzxlz.cn/gtitssfpta.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yongpay.top/gtqddmbcbt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.bjfxy.top/gtpzizbxuo.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.smart0.xyz/gtsbfkrjsk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yueranfly.top/gtqlcsxgty.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shuidangran.top/gtkrhufwex.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.kuanghao11.cn/gtcekskodp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.kuanghao11.cn/gtncfwaeky.html

[A07] 数字转字符串
来源：http://hz.snrcjt.cn/gtrelzpzvn.html

Py:   str(42)
来源：http://hz.0kj1m.cn/gttgznlgbb.html

PHP:  (string) 42; strval(42)
来源：http://hz.ppjwa.cn/gtjlxuhxox.html

JS:   String(42); (42).toString()
来源：http://hz.zhiwuduotai.top/gttqvgiuaq.html

TS:   String(42)
来源：http://hz.wangshuangyany.cn/gtvrjrzplv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.316326.xyz/gtikdvhnwk.html

Go:   strconv.Itoa(42)
来源：http://hz.zhiwuduotai.top/gtfpeaubkv.html

Ruby: 42.to_s
来源：http://hz.ydzc1.top/gtwinglkkh.html

C#:   42.ToString()
来源：http://hz.yvedp.cn/gtvkzwwwrj.html

[A08] 取整与四舍五入
来源：http://hz.ybcxt.top/gtwndqjaud.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xuetiantiany.cn/gtkbbvljno.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cdnleiting.top/gtpzeerowr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhoulong.xyz/gtpyrbrmmb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.nanxinkj.top/gtkkdzpbav.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nwbrower.top/gtevcvgmth.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.fengsongda.top/gtxdnxeadi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.shanyushiyangkeji.top/gtmwhtrwtw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xuetiantiany.cn/gtdfovqyva.html

[A09] 绝对值与最大最小值
来源：http://hz.quarkkingdee.top/gtmxghmiui.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hongshengwenyu.top/gtytaxiemx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tanke756.top/gtzisvyyql.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.gotoacloud.top/gtutmpngcp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.quarkkingdee.top/gtakxqszhi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hfpthk.cn/gtxbiccrvx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.316326.xyz/gtysjurluo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.redwolf501.top/gteztbneqt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.0kj1m.cn/gtxqyxbuhm.html

[A10] 生成随机数
来源：http://hz.dianchejie.cn/gttnnoiqmt.html

Py:   import random; random.randint(1, 100)
来源：http://hz.tianlin.xyz/gtjbpumvxl.html

PHP:  random_int(1, 100);
来源：http://hz.haohaochexian.top/gtkrlozzez.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.52xcode.cn/gttjtbmjvy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.bjfxy.top/gthjllurco.html

Java: new Random().nextInt(100) + 1
来源：http://hz.aibaodan.cn/gtmjocphco.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.fengsongda.top/gtksibbnwj.html

Ruby: rand(1..100)
来源：http://hz.aibaodan.cn/gtpwgfobuh.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuxming.cn/gtbabvjcla.html

[A11] 条件表达式（三元）
来源：http://hz.nwbrower.top/gtrogkcobp.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jinyuanbaomall.cn/gthkjflgev.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.fengsongda.top/gtzbzvfuci.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtbnnpwqab.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtcvmghbtz.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtsgnqwgni.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xinyue.icu/gtehpdmwoa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtzgnadsnt.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtdykbjypf.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhiwuduotai.top/gtldaftffr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.sufxvd.cn/gtgsylhjcr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhoulong.xyz/gtuhltsuys.html

JS:   `Hello, ${name}!`
来源：http://hz.birdmap.top/gtlxudncsc.html

TS:   `Hello, ${name}!`
来源：http://hz.iojbl.cn/gtaiqgrike.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhaomingkeji.xyz/gtbpepxgyc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jyoumei.cn/gtqxnzqhrm.html

Ruby: "Hello, #{name}!"
来源：http://hz.jqgufenzy.top/gtwgixayyz.html

C#:   $"Hello, {name}!"
来源：http://hz.0kj1m.cn/gtmfilsiee.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cucudq.cn/gtiznqcdag.html

Py:   "第一行\n第二行"
来源：http://hz.havefunace.top/gtdkfypwnl.html

PHP:  "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtvdpfrnan.html

JS:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtppsqpykg.html

TS:   "第一行\n第二行"
来源：http://hz.havefunace.top/gtmvzdnqjx.html

Java: "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtzsjmujja.html

Go:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtwsmhwhhh.html

Ruby: "第一行\n第二行"
来源：http://hz.iojbl.cn/gtbsuqnblu.html

C#:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtrxqtlrgy.html

[A14] 注释写法
来源：http://hz.snrcjt.cn/gtenxehdbu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhengqikj.top/gtzltmkeqf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yuxming.cn/gtmpmmiwmy.html

JS:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gttcrhltgs.html


<!-- 参考信息 -->