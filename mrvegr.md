代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.hnqzz.top/gtxancyywx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jlsjyb.cn/gtqtlxmlfv.html

[U84] JS：CommonJS 写法
来源：http://hz.shuidangran.top/gtvlctzpuk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangshuangyany.cn/gtimapsxqm.html

[U85] JS：可选链
来源：http://hz.jinqigfzy.top/gtwwozybrm.html

a?.b?.c
来源：http://hz.jinyuanbaomall.cn/gtvoxeegeh.html

[U86] JS：空值合并
来源：http://hz.hongshengwenyu.top/gtfwfhfznx.html

a ?? b
来源：http://hz.jyoumei.cn/gtznqumaep.html

[U87] JS：解构默认值
来源：http://hz.xylfe.cn/gtoogeopov.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jqgfzy.top/gtmyfpfgta.html

[U88] JS：对象展开合并
来源：http://hz.chenjidiqi.icu/gtqobuodnk.html

{ ...a, ...b }
来源：http://hz.xuanzx.com/gtlyjmzbkg.html

[U89] JS：数组去重
来源：http://hz.xinyue.icu/gteixyabcp.html

[...new Set(arr)]
来源：http://hz.9152youxi.cn/gtljpmevhy.html

[U90] JS：数字数组排序
来源：http://hz.shzxlz.cn/gttwkgnzst.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtrmfrerde.html

[U91] JS：对象键值遍历
来源：http://hz.gaohongyu789.top/gtjosurqwn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgufenzy.top/gtqxtcjjru.html

[U92] JS：深拷贝
来源：http://hz.feifeiyinyue.top/gtptgvjmhj.html

structuredClone(obj)
来源：http://hz.svipenyu.cn/gtrzqynifs.html

[U93] JS：模板字符串
来源：http://hz.redwolf501.top/gtkxipdlea.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gtqwvtrzeu.html

[U94] JS：箭头函数
来源：http://hz.yvedp.cn/gterbwkhlo.html

const double = x => x * 2;
来源：http://hz.pycfn.com/gtqktbfwgt.html

[U95] JS：Promise 包装
来源：http://hz.316326.xyz/gtbqzkmhmg.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtbppgkmgu.html

[U96] JS：async/await 与异常
来源：http://hz.zdqjudy.top/gtxgjlrdqx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtncxslsnn.html

[U97] JS：并发请求
来源：http://hz.xuanzx.com/gtmfiicylo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gthgkrzsmi.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gtsjlxycxk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.52xcode.cn/gtpzasvjqw.html

[U99] JS：事件监听
来源：http://hz.cqqwz.cn/gtkdktadut.html

el.addEventListener("click", e => {})
来源：http://hz.ehwqpu.com/gtyghhmfum.html

[U100] JS：DOM 查询
来源：http://hz.meibo888.top/gtacytxslv.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gtxfycnkeg.html

[U101] JS：classList 操作
来源：http://hz.zdqjudy.top/gtfkkrypwy.html

el.classList.toggle("active")
来源：http://hz.xuanzx.com/gtrwgenicz.html

[U102] JS：本地存储
来源：http://hz.andypj.xyz/gtcwvzgybu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuanzx.com/gtazmvyisk.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtyaknxerw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtwcixthhk.html

[U104] JS：防抖
来源：http://hz.xingfuxueyuan.xyz/gtmpjtthtn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtvydcjkjn.html

[U105] JS：节流
来源：http://hz.bjfxy.top/gtbmistqxf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yvedp.cn/gtcijfktze.html

[U106] JS：日期格式化
来源：http://hz.shanyushiyangkeji.top/gthpeujpmr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sweek.top/gteuovdagf.html

[U107] JS：数字千分位
来源：http://hz.ybcxt.top/gtaehbuuqj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnqzz.top/gtzctmvtnf.html

[U108] JS：随机整数
来源：http://hz.jianghu66.top/gtvtadzflt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.wangshuangyany.cn/gtnljjltqh.html

[U109] JS：数组分组
来源：http://hz.jinqigufen.top/gtwklwpagv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtwnihfwyx.html

[U110] JS：数组分块
来源：http://hz.xuanzx.com/gtisaobkac.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhongyouzk.top/gtkdqqqads.html

[U111] JS：对象转 Map
来源：http://hz.iojbl.cn/gtfkvzrryy.html

new Map(Object.entries(obj))
来源：http://hz.yj202588.top/gtadilrxwo.html

[U112] JS：字符串补位
来源：http://hz.hongshengwenyu.top/gtbyqerhmt.html

"7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtdfspfzuq.html

[U113] JS：正则替换全部
来源：http://hz.cashguo.top/gtbamnwcfv.html

s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtglvzxxiz.html

[U114] JS：JSON 深比较
来源：http://hz.ppjwa.cn/gtvvyniyfv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtkmnmpyru.html

[U115] JS：生成 UUID
来源：http://hz.svipenyu.cn/gtrdzwzpzf.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtfdtxddhs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ivvv.top/gtunbbkryi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenzaomai.com/gticjhebvk.html

[U117] JS：单元测试
来源：http://hz.yanxiufei.cn/gtshtjkvkf.html

npm i -D vitest;  npx vitest
来源：http://hz.svipenyu.cn/gtqakpfnrt.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtytphvzfm.html

npm i -D vite;  npx vite
来源：http://hz.zhixingplan.top/gtzgmuppvb.html

[U119] JS：生产构建
来源：http://hz.yueranfly.top/gtaqkcabul.html

npx vite build
来源：http://hz.aizwys.cn/gtjnsfopqb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nanxinkj.top/gtixstqogy.html

import.meta.env.VITE_API_URL
来源：http://hz.c1oappe.top/gtempnavwe.html

================================================================================
来源：http://hz.jqgfzy.top/gtyceojmzw.html

统计汇总
来源：http://hz.gogol.net.cn/gtscrseotz.html

================================================================================
来源：http://hz.cucudq.cn/gthhfuolsz.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtuggslhzl.html

Python ......... 252
来源：http://hz.sweek.top/gtowiytswl.html

PHP ............ 252
来源：http://hz.9152youxi.cn/gtmjlpaflu.html

JavaScript ..... 252
来源：http://hz.chenzaomai.com/gtlhfjbttz.html

TypeScript ..... 212
来源：http://hz.yuxming.cn/gthpemyngy.html

Java ........... 212
来源：http://hz.xziqi.cn/gtqlsvkfwx.html

Go ............. 212
来源：http://hz.vqdsnc.cn/gthqkolhch.html

Ruby ........... 212
来源：http://hz.dianchejie.cn/gtwehzaewn.html

C# ............. 212
来源：http://hz.gaohongyu789.top/gtrfyhqkcc.html

C .............. 30
来源：http://hz.hysaishi.cn/gtumabrguf.html

C++ ............ 30
来源：http://hz.zhixingplan.top/gtszojmqmq.html

SQL ............ 90
来源：http://hz.nwbrower.top/gtcltetlgx.html

Bash ........... 80
来源：http://hz.xinyue.icu/gtqslacomo.html

Kotlin ......... 15
来源：http://hz.zhixingplan.top/gtmlcjptpw.html

Swift .......... 15
来源：http://hz.0kj1m.cn/gtopnwlckf.html

Lua ............ 10
来源：http://hz.gzhubu.top/gtjcxjalib.html

Perl ........... 10
来源：http://hz.jyoumei.cn/gtyqmjwacd.html

Scala .......... 10
来源：http://hz.shuidangran.top/gtugaobrxg.html

------------------------------------
来源：http://hz.yuanzhike.top/gtjkmgxhqv.html

合计 ........... 2106 条
来源：http://hz.cheryme.top/gtxfaxbmkj.html

按章节统计：
来源：http://hz.jyoumei.cn/gtyhkbwyyu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gtpbeujltf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtisvhxkgx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtoplmaqnp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtnmmdgzgm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnxiangtu.top/gtajhldubk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtucqyivid.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtojicxwnt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtuugdichd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtkoajuszk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtbzokhklk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtleymwdzp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtffkkrtyi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtotrmlekd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zdqjudy.top/gtqetroywj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtxvdobfvm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtwlyrsrsi.html

Q SQL 专题                              90
来源：http://hz.xinyue.icu/gtaxigegsc.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtzfjxxkyc.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtpfrxbofs.html

T 其他语言补充                          60
来源：http://hz.316326.xyz/gtjrvidkuw.html

U 高频实用片段                         120
来源：http://hz.jiagoushi.top/gtrwjdvvyk.html

------------------------------------
来源：http://hz.yonumen.top/gtdgriedya.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtegnkatzn.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gtpkbwcdda.html

使用提醒
来源：http://hz.nwbrower.top/gtgmrhbwqn.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtcaaxtnyy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hywenlv.cn/gtjgbdbizj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jqgufenzy.top/gtpbxgzmcn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jqgfzy.top/gtvdhjcgoy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sweek.top/gtefwdeupw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ywan-chungtsiang.top/gtahhmculj.html

—— 文件结束 ——
来源：http://hz.hnxiangtu.top/gttxgberuw.html

================================================================================
来源：http://hz.nwbrower.top/gtrjepkewx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhijiandao.cn/gtetkbuhro.html

Common Programming Examples Cheat Book
来源：http://hz.gzhubu.top/gtqmghlxaj.html

================================================================================
来源：http://hz.yvedp.cn/gtnzegoaxs.html

【收录内容】
来源：http://hz.jiagoushi.top/gtkdperizq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.haohaochexian.top/gtndyzqciy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.c1oappe.top/gtfnjvimpp.html

SQL · Bash · C · C++
来源：http://hz.wangdashe.top/gthgivndnu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sweek.top/gteuunzzhp.html

【使用说明】
来源：http://hz.jinghuilouyu.cn/gtaplxiyje.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sufxvd.cn/gtpnmafbwu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj202588.top/gtyyzvscrk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtudkozgvw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yangfankeji.com/gteqrtsoxp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.havefunace.top/gtilwjljgc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.guannengcc.top/gtabpzxadb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.kuanghao11.cn/gtuchvymqj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tanke756.top/gttoyjlqpr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cdnleiting.top/gtanpzozjm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fengsongda.top/gtkosqnqus.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ywan-chungtsiang.top/gtnhfokawh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.vqdsnc.cn/gtegcfavtf.html

【文件统计】
来源：http://hz.zhongyouzk.top/gtghauwdrb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hnqzz.top/gtllexaxxm.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtougfubqg.html

目  录
来源：http://hz.havefunace.top/gtgnhoirpu.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtvefdvpna.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.guannengcc.top/gtrkymmint.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtqzxipjrb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtfztulvfq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtussuxkik.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.9152youxi.cn/gtavdzfojz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtfnhgvoub.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtgghtvmrw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.snrcjt.cn/gtmyvqsggg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtxaebwhhn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shuidangran.top/gthgdxapvd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtkpelwxae.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtqxuraaag.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtcgnnqbro.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yuxming.cn/gtgkhldmni.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtwiflzkul.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtzfbzmsxy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yanxiufei.cn/gtptgkepgs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sweek.top/gtjnyqaouz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yvedp.cn/gtgkbbyugi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hammf.cn/gtmtaxsjqn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gthuvkxroc.html

================================================================================
来源：http://hz.sysykeji.top/gtcnsawhdo.html

A. 基础语法与类型
来源：http://hz.ybcxt.top/gthjbvyfej.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpppduvba.html

[A01] Hello World
来源：http://hz.mhx1999.top/gtpvdglarg.html

Py:   print("Hello, World!")
来源：http://hz.ydjk.org.cn/gtbahyrato.html

PHP:  echo "Hello, World!";
来源：http://hz.guannengcc.top/gtqelzhbxq.html

JS:   console.log("Hello, World!");
来源：http://hz.hfpthk.cn/gtvtodlklk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gotoacloud.top/gtcyxxpagf.html

Java: System.out.println("Hello, World!");
来源：http://hz.sufxvd.cn/gtmtdddugu.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.snrcjt.cn/gtirgjiccp.html

Ruby: puts "Hello, World!"
来源：http://hz.dashuyun.cn/gtlzejstbo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhijiandao.cn/gtyqioxote.html

[A02] 变量声明与赋值
来源：http://hz.zhoulong.xyz/gtasnenisn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtqpttlngw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ybcxt.top/gtahglcagx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sweek.top/gtochpvnod.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.aizwys.cn/gtcffdddvl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.guowangkeji.top/gtdxuqbrnh.html

Go:   name := "Alex"; age := 20
来源：http://hz.yuanzhike.top/gtnosnzwyr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhoulong.xyz/gtpqgfdmwl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtnrwlaihu.html

[A03] 常量定义
来源：http://hz.hammf.cn/gtwaavfgpq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhongyouzk.top/gtjwrouele.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258888.top/gtcfdcikyw.html

JS:   const PI = 3.14159;
来源：http://hz.ybcxt.top/gtiabbevlc.html

TS:   const PI: number = 3.14159;
来源：http://hz.hfpthk.cn/gtctresssc.html

Java: static final double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtmpzjzjdp.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangtech.top/gtoqggxcqp.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtpbfgizxd.html

C#:   const double PI = 3.14159;
来源：http://hz.havefunace.top/gtbozfjsni.html

[A04] 判断变量类型
来源：http://hz.sysykeji.top/gtgqivajhl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnqzz.top/gtuspvuquk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shuidangran.top/gtbqzrjhen.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.chenzaomai.com/gtldqvjdrt.html

TS:   typeof x; x instanceof Date
来源：http://hz.jqgfzy.top/gtlakufwst.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.chenzaomai.com/gtwsdsxwxs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.dianchejie.cn/gtmacflzei.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.316326.xyz/gtlflqpyxq.html

C#:   x.GetType().Name; x is int
来源：http://hz.iojbl.cn/gtbhidqpxz.html

[A05] 整数除法与取模
来源：http://hz.mhx1999.top/gtphqmaofq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xuetiantiany.cn/gtdcfkaaxb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yanxiufei.cn/gtfvupidkg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.0kj1m.cn/gtvcruachr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.redwolf501.top/gtnmeqbrxv.html

Java: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtsrkmltnc.html

Go:   7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtvimrleaj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtqqekesok.html

C#:   7 / 2; 7 % 2
来源：http://hz.sweek.top/gtmxakldbl.html

[A06] 字符串转数字
来源：http://hz.jinqigufen.top/gtjegvheyn.html

Py:   int("42"); float("3.14")
来源：http://hz.kuanghao11.cn/gtourhyhec.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhengqikj.top/gtikyspact.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.mhx1999.top/gtsnqfcspo.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.vqdsnc.cn/gtuskddisg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shanyushiyangkeji.top/gtvsmreefd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shangyingyoupin.top/gtwazaerce.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ydjk.org.cn/gtzaqecbzh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.nanxinkj.top/gtgodgepdr.html

[A07] 数字转字符串
来源：http://hz.havefunace.top/gtfxfllzxo.html

Py:   str(42)
来源：http://hz.zhijiandao.cn/gtycidhhvt.html

PHP:  (string) 42; strval(42)
来源：http://hz.xingfuxueyuan.xyz/gtisdiggix.html

JS:   String(42); (42).toString()
来源：http://hz.sxryk.cn/gtnqnhpzsf.html

TS:   String(42)
来源：http://hz.0kj1m.cn/gttcuwezmb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhongyouzk.top/gtjounyrwp.html

Go:   strconv.Itoa(42)
来源：http://hz.jinghuilouyu.cn/gtogfgyhua.html

Ruby: 42.to_s
来源：http://hz.ydjk.org.cn/gtthsvdtqu.html

C#:   42.ToString()
来源：http://hz.birdmap.top/gtrtyrcdvq.html

[A08] 取整与四舍五入
来源：http://hz.c1oappe.top/gteyppduos.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ppjwa.cn/gteqgnaxsj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.wangdashe.top/gtkqajffzy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hnxiangtu.top/gtqxeikkoz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigufen.top/gtmswduxcy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hongshengwenyu.top/gtbkeanryp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.vqdsnc.cn/gtnsmqnhfu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sxryk.cn/gtgptiohde.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sxryk.cn/gtzhhxlfaq.html

[A09] 绝对值与最大最小值
来源：http://hz.tian-w.cn/gtjuiuiciw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aizwys.cn/gtowfbahyh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gzhubu.top/gtmnpprzsl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nanxuanxn.top/gtmfpjtcmk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jqgfzy.top/gtdinxcciu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.wangshuangyany.cn/gtiefdptwv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.ywan-chungtsiang.top/gtpbasvtmk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xinyue.icu/gtdhoasdkm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xuetiantiany.cn/gtmzwhlqxa.html

[A10] 生成随机数
来源：http://hz.xuanzx.com/gtpscjldwl.html

Py:   import random; random.randint(1, 100)
来源：http://hz.aibaodan.cn/gtjvnsukqg.html

PHP:  random_int(1, 100);
来源：http://hz.ppjwa.cn/gtnqzyyfma.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj20258888.top/gtqskwipfr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuanzhike.top/gtaxktcjfc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.daria6918.cn/gtzllfkpha.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.cucudq.cn/gtbcqlihaj.html

Ruby: rand(1..100)
来源：http://hz.cucudq.cn/gtppbwroas.html

C#:   new Random().Next(1, 101)
来源：http://hz.xylfe.cn/gtgrhafxrv.html

[A11] 条件表达式（三元）
来源：http://hz.smart0.xyz/gteffprmbo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yj20258.top/gtiqblnkio.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jqgfzy.top/gturuvzppi.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtbhpectyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtjucfljrz.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtegjofbkl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jqgufenzy.top/gttmmgmonk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtkfyqlmbn.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gtdsyqetua.html

[A12] 字符串插值 / 格式化
来源：http://hz.haohaochexian.top/gtqkzbzuvm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.ydjk.org.cn/gteuezauis.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.bjfxy.top/gthdqiabco.html

JS:   `Hello, ${name}!`
来源：http://hz.kuanghao11.cn/gtgorqpxky.html

TS:   `Hello, ${name}!`
来源：http://hz.shzxlz.cn/gtkcjxouxs.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jiagoushi.top/gtnfktxrfm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.quarkkingdee.top/gtehncabhx.html

Ruby: "Hello, #{name}!"
来源：http://hz.shzxlz.cn/gtzjejvcfn.html

C#:   $"Hello, {name}!"
来源：http://hz.yj20258.top/gtumywyttn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.aibaodan.cn/gtqizrufyu.html

Py:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtnfspvrxc.html

PHP:  "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtheudlriv.html

JS:   "第一行\n第二行"
来源：http://hz.mhx1999.top/gtzczzyvyy.html

TS:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtcttujvno.html

Java: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtfgqnvsor.html

Go:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtcmyorqbz.html

Ruby: "第一行\n第二行"
来源：http://hz.xuetiantiany.cn/gtkbtvzbyo.html

C#:   "第一行\n第二行"
来源：http://hz.hfpthk.cn/gttgptjpac.html


<!-- 参考信息 -->