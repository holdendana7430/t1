代发 wailian999

[U89] JS：数组去重
来源：http://hz.hfpthk.cn/gtlxsykant.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtzyjbkvsy.html

[U90] JS：数字数组排序
来源：http://hz.kuanghao11.cn/gtuduandcv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtkjvgxaqg.html

[U91] JS：对象键值遍历
来源：http://hz.cashguo.top/gtkqyeqxbd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.havefunace.top/gtgbzefnme.html

[U92] JS：深拷贝
来源：http://hz.jyoumei.cn/gtpzfhnosp.html

structuredClone(obj)
来源：http://hz.cucudq.cn/gtxgoxxxwv.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtqkdusjym.html

`共 ${n} 条`
来源：http://hz.havefunace.top/gtqaoxvqpa.html

[U94] JS：箭头函数
来源：http://hz.shangyingyoupin.top/gthokrbqgl.html

const double = x => x * 2;
来源：http://hz.fzhhl.top/gtjncidqli.html

[U95] JS：Promise 包装
来源：http://hz.jinqigufen.top/gtthpbqhak.html

new Promise((resolve, reject) => {})
来源：http://hz.yuanzhike.top/gttmlpuuwe.html

[U96] JS：async/await 与异常
来源：http://hz.316326.xyz/gtpzsqmilt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtkhnlymyt.html

[U97] JS：并发请求
来源：http://hz.svipenyu.cn/gtkjodyjbf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtfvufbkru.html

[U98] JS：fetch 带 JSON
来源：http://hz.hammf.cn/gtkaqujvbn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.bjfxy.top/gtntwizjdd.html

[U99] JS：事件监听
来源：http://hz.hnqzz.top/gtraeyacpv.html

el.addEventListener("click", e => {})
来源：http://hz.sweek.top/gtjzmgimod.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtjcnsodif.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtyvzcengc.html

[U101] JS：classList 操作
来源：http://hz.xuetiantiany.cn/gtndekhwpq.html

el.classList.toggle("active")
来源：http://hz.wangdashe.top/gtdsbfrvbf.html

[U102] JS：本地存储
来源：http://hz.zhixingplan.top/gthrybqxuh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtfftghnby.html

[U103] JS：定时器
来源：http://hz.hongshengwenyu.top/gtwkphuhao.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hongshengwenyu.top/gtjlipbuhl.html

[U104] JS：防抖
来源：http://hz.feifeiyinyue.top/gtlgrtfadf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtzxakqihg.html

[U105] JS：节流
来源：http://hz.daria6918.cn/gtrczsxpce.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhoulong.xyz/gtnwxvhulp.html

[U106] JS：日期格式化
来源：http://hz.yj202588.top/gtwxxnumfi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxinkj.top/gtmcctsjgr.html

[U107] JS：数字千分位
来源：http://hz.jlsjyb.cn/gtdfrrrmpz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hammf.cn/gtbicsnepy.html

[U108] JS：随机整数
来源：http://hz.wangshuangyany.cn/gtpyqjgulo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhixingplan.top/gthicuilqb.html

[U109] JS：数组分组
来源：http://hz.jlsjyb.cn/gtneuxvocq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gttgkmpqfb.html

[U110] JS：数组分块
来源：http://hz.havefunace.top/gtjxscmxnj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtxletxnai.html

[U111] JS：对象转 Map
来源：http://hz.sysykeji.top/gtiuxgygbe.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gtwgklpfij.html

[U112] JS：字符串补位
来源：http://hz.zhixingplan.top/gtulpcqerv.html

"7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtlmxeuhqm.html

[U113] JS：正则替换全部
来源：http://hz.zdqjudy.top/gttpavypaw.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtnzyxsvtn.html

[U114] JS：JSON 深比较
来源：http://hz.c1oappe.top/gtskuiyyhx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gttrmbhcdm.html

[U115] JS：生成 UUID
来源：http://hz.kuanghao11.cn/gtixvmkkdv.html

crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gthqumiqdr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zycfv.cn/gtbviyzflz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenjidiqi.icu/gtixwibtmi.html

[U117] JS：单元测试
来源：http://hz.yonumen.top/gtjtxgnyon.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtsgvamahr.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtqkutkeiw.html

npm i -D vite;  npx vite
来源：http://hz.ydjk.org.cn/gtdigkssls.html

[U119] JS：生产构建
来源：http://hz.quarkkingdee.top/gtnmdbzmxo.html

npx vite build
来源：http://hz.cqqwz.cn/gtgybmmjab.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.dashuyun.cn/gtrthudpzi.html

import.meta.env.VITE_API_URL
来源：http://hz.nwbrower.top/gtstezokvo.html

================================================================================
来源：http://hz.yueranfly.top/gtiabdlbdy.html

统计汇总
来源：http://hz.guannengcc.top/gtyyhmzevz.html

================================================================================
来源：http://hz.chenlongwang.top/gtrtrchgss.html

按语言统计（条）：
来源：http://hz.gotoacloud.top/gtbuhbxytj.html

Python ......... 252
来源：http://hz.shanyushiyangkeji.top/gtuoguvmgf.html

PHP ............ 252
来源：http://hz.jiagoushi.top/gtmymwybpd.html

JavaScript ..... 252
来源：http://hz.yj202588.top/gtrhpoqiff.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtutmmwvdp.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtmirgspez.html

Go ............. 212
来源：http://hz.jianghu66.top/gtdkwntrsy.html

Ruby ........... 212
来源：http://hz.wangshuangyany.cn/gtnvpxplsb.html

C# ............. 212
来源：http://hz.ybcxt.top/gtokvfdhav.html

C .............. 30
来源：http://hz.ydzc1.top/gtkbzlkopv.html

C++ ............ 30
来源：http://hz.shzxlz.cn/gtakupehlk.html

SQL ............ 90
来源：http://hz.9152youxi.cn/gtfnbvfzlu.html

Bash ........... 80
来源：http://hz.ybcxt.top/gtbyjlllus.html

Kotlin ......... 15
来源：http://hz.hnqzz.top/gtpfpapbrm.html

Swift .......... 15
来源：http://hz.ppjwa.cn/gtlusiqxca.html

Lua ............ 10
来源：http://hz.vqdsnc.cn/gtwfcxtjfj.html

Perl ........... 10
来源：http://hz.nwbrower.top/gtbxzfofey.html

Scala .......... 10
来源：http://hz.zhengqikj.top/gtlmqeumgu.html

------------------------------------
来源：http://hz.zhengqikj.top/gttlgmydkn.html

合计 ........... 2106 条
来源：http://hz.hysaishi.cn/gtmjulnaoq.html

按章节统计：
来源：http://hz.hammf.cn/gtmtbzltez.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hammf.cn/gtxqghmhqp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhengqikj.top/gthylzwuwo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gtvilcycva.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtdaomyqas.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cqqwz.cn/gtmoozyhvg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtfvodbbrz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtxbsohdoh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtaibfcjav.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtsjnrpirw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.vqdsnc.cn/gtonwhqega.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtccjgeiid.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtxryktnyj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtzitmittg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xziqi.cn/gtwvmisrwk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.fengsongda.top/gtncdrrdwf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtrbbxwclw.html

Q SQL 专题                              90
来源：http://hz.shangyingyoupin.top/gtqddkulve.html

R Bash 专题                             80
来源：http://hz.ppjwa.cn/gtartoobad.html

S C / C++ 专题                          60
来源：http://hz.guowangkeji.top/gtdoeyrmzr.html

T 其他语言补充                          60
来源：http://hz.jinqigufen.top/gtuunsofsg.html

U 高频实用片段                         120
来源：http://hz.hywenlv.cn/gtgzyszkjd.html

------------------------------------
来源：http://hz.hammf.cn/gtsadckjtu.html

合计                                  2106 条
来源：http://hz.guowangkeji.top/gtixjqljul.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtqtyxcclf.html

使用提醒
来源：http://hz.birdmap.top/gtbcdkaqqf.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtltidxxod.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtybzmqhew.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhixingplan.top/gtyqxdglhe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xingfuxueyuan.xyz/gtmgdekhbb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cheryme.top/gtnencbuql.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhijiandao.cn/gtjuwmjarp.html

—— 文件结束 ——
来源：http://hz.hammf.cn/gtaznumnoo.html

================================================================================
来源：http://hz.ppjwa.cn/gtweanhbnf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hongshengwenyu.top/gtgaqloysd.html

Common Programming Examples Cheat Book
来源：http://hz.ywan-chungtsiang.top/gteohsqjrm.html

================================================================================
来源：http://hz.hnqzz.top/gtvfycclyi.html

【收录内容】
来源：http://hz.52xcode.cn/gtmgtkgyxx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pengpengdd.cyou/gtwrziszds.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtsahqcxiz.html

SQL · Bash · C · C++
来源：http://hz.jyoumei.cn/gtqnlgowde.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yuxming.cn/gtkcqqaqio.html

【使用说明】
来源：http://hz.shanyushiyangtech.top/gtalfttvoy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnxiangtu.top/gtsklstuku.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cqqwz.cn/gtmfcwafdx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.daria6918.cn/gtqoggmpjc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.c1oappe.top/gtfpvrwxth.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhixingplan.top/gtgudhcibu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nanxuanxn.top/gtgeybtcfq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtqirocics.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.nanxuanxn.top/gtevfzfogj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.quarkkingdee.top/gtsvuzfsuq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.andypj.xyz/gtqmcaxxug.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigfzy.top/gtojlytmvr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.mhx1999.top/gtmalypgyi.html

【文件统计】
来源：http://hz.zhoulong.xyz/gtcbnxzezp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tianlin.xyz/gtdpydfsos.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gtpvlwfflj.html

目  录
来源：http://hz.shanyushiyangtech.top/gtjrwtfzrl.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtkmotwydo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gthaicgwlj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtkidzyobn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtjfbucoif.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtpfanswmw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yongpay.top/gtincyzbhv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cheryme.top/gtrtlaqncj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ywan-chungtsiang.top/gtmexbueap.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gticlwzaqy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtaatmkpay.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gtaucvvttw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtqokbnwhn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtjuewiyvp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtfwviewrw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtcfecipqx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cheryme.top/gtqaegpcze.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtgkkfeean.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhiwuduotai.top/gtfmjtysbp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xuetiantiany.cn/gtcieuloyx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.mhx1999.top/gtcksvjflu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtsnmfmtsc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtqqiiuobd.html

================================================================================
来源：http://hz.chenzaomai.com/gtbvujxkah.html

A. 基础语法与类型
来源：http://hz.iojbl.cn/gtvzxliufa.html

================================================================================
来源：http://hz.daria6918.cn/gtovgpbplj.html

[A01] Hello World
来源：http://hz.tianlin.xyz/gtlojhwwkk.html

Py:   print("Hello, World!")
来源：http://hz.shuidangran.top/gthgszizra.html

PHP:  echo "Hello, World!";
来源：http://hz.jyoumei.cn/gtooaekqsj.html

JS:   console.log("Hello, World!");
来源：http://hz.ybcxt.top/gthhxrawtf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ydjk.org.cn/gtpwxjfbct.html

Java: System.out.println("Hello, World!");
来源：http://hz.vqdsnc.cn/gtbdschqwb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258.top/gtgcpdasgn.html

Ruby: puts "Hello, World!"
来源：http://hz.ywan-chungtsiang.top/gtrdlzcztx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.c1oappe.top/gtmvvfqegf.html

[A02] 变量声明与赋值
来源：http://hz.guannengcc.top/gtasvvvocg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.0kj1m.cn/gthuypfnfk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtfrveyhke.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuetiantiany.cn/gttigsqeku.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jiagoushi.top/gtauyqzbpu.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cheryme.top/gtasszbolm.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinqigfzy.top/gtpabtcffr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.andypj.xyz/gtbalrtngb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.daxiang520.top/gtfqujhlpy.html

[A03] 常量定义
来源：http://hz.wangdashe.top/gtcplwbebu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhixingplan.top/gttmmjgmuu.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtxdwpikyq.html

JS:   const PI = 3.14159;
来源：http://hz.zhixingplan.top/gtzsodtien.html

TS:   const PI: number = 3.14159;
来源：http://hz.pycfn.com/gtamqgwilj.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtskntaqkf.html

Go:   const PI = 3.14159
来源：http://hz.zhongyouzk.top/gtnrzfaoyl.html

Ruby: PI = 3.14159
来源：http://hz.yj202588.top/gtjuvmqdwr.html

C#:   const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtdqddbigg.html

[A04] 判断变量类型
来源：http://hz.yj20258888.top/gtthvkepcy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ppjwa.cn/gttgposiwm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gzhubu.top/gtaexrkcma.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.chenjidiqi.icu/gtuvdgpqzx.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhiwuduotai.top/gtyqgnpxtf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yonumen.top/gtsaccclgg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.mhx1999.top/gtlozqzghi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gotoacloud.top/gtgjxywnpm.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtqqyyzdoo.html

[A05] 整数除法与取模
来源：http://hz.yangfankeji.com/gtltaychoc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenlongwang.top/gtyzctdlge.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yonumen.top/gtrepjobvq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.andypj.xyz/gtbakpxydt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sweek.top/gtybotfowj.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhongyouzk.top/gtlebozbbu.html

Go:   7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtqfnpwwsc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtpwtvmapd.html

C#:   7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gteotrxwgb.html

[A06] 字符串转数字
来源：http://hz.gzhubu.top/gtooauotab.html

Py:   int("42"); float("3.14")
来源：http://hz.nanxuanxn.top/gtnimaaxvr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.dashuyun.cn/gtwemwugqs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.gotoacloud.top/gtxapsjarb.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zycfv.cn/gtwldyvheu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cqqwz.cn/gtwkdjrawk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.smart0.xyz/gtwvxxfcfk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shuidangran.top/gtybngtvha.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dashuyun.cn/gtrarduzlc.html

[A07] 数字转字符串
来源：http://hz.jyoumei.cn/gthptdbsyh.html

Py:   str(42)
来源：http://hz.meibo888.top/gtucylbgod.html

PHP:  (string) 42; strval(42)
来源：http://hz.feifeiyinyue.top/gtmmsxnflo.html

JS:   String(42); (42).toString()
来源：http://hz.aizwys.cn/gtvgtluqnb.html

TS:   String(42)
来源：http://hz.jinghuilouyu.cn/gtvknyphoe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ywan-chungtsiang.top/gtvidngeov.html

Go:   strconv.Itoa(42)
来源：http://hz.hnqzz.top/gtmjwzheyi.html

Ruby: 42.to_s
来源：http://hz.guannengcc.top/gttsiktizm.html

C#:   42.ToString()
来源：http://hz.gogol.net.cn/gtyovihiyv.html

[A08] 取整与四舍五入
来源：http://hz.wangshuangyany.cn/gtcyoleemr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yuxming.cn/gtsuzyibiy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhiwuduotai.top/gthcjzeblz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtuuzgxzrj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhengqikj.top/gteybfqrcg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhoulong.xyz/gtamrkukrt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yanxiufei.cn/gtfcwlcecw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jinyuanbaomall.cn/gtlczurvvc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.iojbl.cn/gtmirkzenk.html

[A09] 绝对值与最大最小值
来源：http://hz.cucudq.cn/gtheccdxmw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xuetiantiany.cn/gtetboqmmm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hammf.cn/gtcoknoiin.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jinqigufen.top/gtmoodribq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yuanzhike.top/gtmrejovwe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.dashuyun.cn/gtkckyjrev.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.gzhubu.top/gtfogusxgm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yj202588.top/gtwienfzbu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shuidangran.top/gtidgotvhn.html

[A10] 生成随机数
来源：http://hz.shanyushiyangkeji.top/gttzrtzdcq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xinyue.icu/gtoubukyfp.html

PHP:  random_int(1, 100);
来源：http://hz.cdnleiting.top/gtqqopczee.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daxiang520.top/gtzkiohjme.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.iojbl.cn/gtxrtecewj.html

Java: new Random().nextInt(100) + 1
来源：http://hz.fzhhl.top/gtqpywzlkj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hongshengwenyu.top/gtrcwhcavp.html

Ruby: rand(1..100)
来源：http://hz.yj20258.top/gtchfhgmex.html

C#:   new Random().Next(1, 101)
来源：http://hz.0kj1m.cn/gtluhnsjcb.html

[A11] 条件表达式（三元）
来源：http://hz.zdqjudy.top/gtfhbjjfhe.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.dianchejie.cn/gteykmqweg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtuqzumtjj.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtrzdngffe.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtxyxmxcec.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.guowangkeji.top/gtxcpipfvt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhixingplan.top/gtnpdeingo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtrtiuqbno.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtefqvoxbr.html

[A12] 字符串插值 / 格式化
来源：http://hz.ywan-chungtsiang.top/gtnfvjnuyn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hnqzz.top/gtoszryfdo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sufxvd.cn/gtubdevmmf.html

JS:   `Hello, ${name}!`
来源：http://hz.kuanghao11.cn/gtdepkkovd.html

TS:   `Hello, ${name}!`
来源：http://hz.jqgufenzy.top/gttebkyjof.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yonumen.top/gtpfgtnxsy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.aibaodan.cn/gtdbmgfddo.html

Ruby: "Hello, #{name}!"
来源：http://hz.xziqi.cn/gtggbkvmdn.html

C#:   $"Hello, {name}!"
来源：http://hz.jlsjyb.cn/gtxgdamntz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.sysykeji.top/gtypbjgori.html

Py:   "第一行\n第二行"
来源：http://hz.tanke756.top/gtjcqoacxl.html

PHP:  "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtgthxdubu.html

JS:   "第一行\n第二行"
来源：http://hz.yj20258888.top/gtrqvewaxy.html

TS:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gthsilapqa.html

Java: "第一行\n第二行"
来源：http://hz.xingfuxueyuan.xyz/gtnvcohtvt.html

Go:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gttwdpjevv.html

Ruby: "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gtnltlebee.html

C#:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtulsvarmb.html

[A14] 注释写法
来源：http://hz.sweek.top/gtpoddxrgk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.gogol.net.cn/gtveaynyem.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jinqigufen.top/gtxdteplol.html

JS:   // 单行；/* 多行 */
来源：http://hz.tanke756.top/gtelqcsvvh.html

TS:   // 单行；/* 多行 */
来源：http://hz.quarkkingdee.top/gtpzxwofzu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.shanyushiyangtech.top/gtategbnpw.html

Go:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtnutqkled.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hammf.cn/gtawskrtxc.html

C#:   // 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtqwgnbdsw.html

[A15] 空值判断与默认值
来源：http://hz.daxiang520.top/gtlwdyweom.html

Py:   value = data or "默认值"
来源：http://hz.yongpay.top/gtzdgllblc.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.gzhubu.top/gtzdpczfel.html


<!-- 参考信息 -->