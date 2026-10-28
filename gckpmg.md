代发 wailian999

[U85] JS：可选链
来源：http://hz.snrcjt.cn/gtfogybkwe.html

a?.b?.c
来源：http://hz.fengsongda.top/gtihwhgmyy.html

[U86] JS：空值合并
来源：http://hz.ydjk.org.cn/gtrdcvjyzu.html

a ?? b
来源：http://hz.gaohongyu789.top/gtifijsfmn.html

[U87] JS：解构默认值
来源：http://hz.shuidangran.top/gtlkdypieu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinqigfzy.top/gtabgpabch.html

[U88] JS：对象展开合并
来源：http://hz.ydzc1.top/gtxjfbduuc.html

{ ...a, ...b }
来源：http://hz.ydjk.org.cn/gtqifeblnr.html

[U89] JS：数组去重
来源：http://hz.andypj.xyz/gtwnpxmcld.html

[...new Set(arr)]
来源：http://hz.cheryme.top/gtqadkwzpu.html

[U90] JS：数字数组排序
来源：http://hz.dashuyun.cn/gtwtcersdy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtxpuhzqoq.html

[U91] JS：对象键值遍历
来源：http://hz.gogol.net.cn/gtfeucwdvi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.svipenyu.cn/gttxfabyue.html

[U92] JS：深拷贝
来源：http://hz.yvedp.cn/gtzmvhdfzm.html

structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtvmzgmquv.html

[U93] JS：模板字符串
来源：http://hz.nwbrower.top/gtiypzctkh.html

`共 ${n} 条`
来源：http://hz.guannengcc.top/gtxnnrksfg.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gturzzxmbn.html

const double = x => x * 2;
来源：http://hz.zycfv.cn/gtxzstfaef.html

[U95] JS：Promise 包装
来源：http://hz.shzxlz.cn/gtyozjcpee.html

new Promise((resolve, reject) => {})
来源：http://hz.tanke756.top/gtayyoonql.html

[U96] JS：async/await 与异常
来源：http://hz.snrcjt.cn/gtdidcutbb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtccoitwkm.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtalzaieqr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtutkadlpc.html

[U98] JS：fetch 带 JSON
来源：http://hz.jqgfzy.top/gtecarjsun.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenzaomai.com/gtlybedzfu.html

[U99] JS：事件监听
来源：http://hz.fengsongda.top/gtpprwmzzm.html

el.addEventListener("click", e => {})
来源：http://hz.hongshengwenyu.top/gtszywpiov.html

[U100] JS：DOM 查询
来源：http://hz.pycfn.com/gtxfgjxfkt.html

document.querySelector(".item")
来源：http://hz.andypj.xyz/gtfbjrhjij.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtqsdmhhxg.html

el.classList.toggle("active")
来源：http://hz.ivvv.top/gtwavkxtge.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtfbeclkya.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ywan-chungtsiang.top/gtrwjhnyok.html

[U103] JS：定时器
来源：http://hz.xinyue.icu/gtwyxummlv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gotoacloud.top/gtuzugxede.html

[U104] JS：防抖
来源：http://hz.yueranfly.top/gtwlwelitl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtfpzrlwcn.html

[U105] JS：节流
来源：http://hz.redwolf501.top/gtjlkyjlcy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xziqi.cn/gthhdqnaqq.html

[U106] JS：日期格式化
来源：http://hz.tanke756.top/gtlumjhbif.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gtlhnpfetv.html

[U107] JS：数字千分位
来源：http://hz.svipenyu.cn/gtbrmobjxq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yangfankeji.com/gtqglkbitb.html

[U108] JS：随机整数
来源：http://hz.nanxuanxn.top/gtlknisuzz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gttxidkrok.html

[U109] JS：数组分组
来源：http://hz.ydzc1.top/gteiixxbgl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtaofqwdlo.html

[U110] JS：数组分块
来源：http://hz.yj202588.top/gtsnwzpbxv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yueranfly.top/gtwukksrmo.html

[U111] JS：对象转 Map
来源：http://hz.ywan-chungtsiang.top/gtfiqjmhjb.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtwyziaqtz.html

[U112] JS：字符串补位
来源：http://hz.havefunace.top/gttkqtzprz.html

"7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gttarxpdyc.html

[U113] JS：正则替换全部
来源：http://hz.hfpthk.cn/gtlrckjrcu.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtxeastlod.html

[U114] JS：JSON 深比较
来源：http://hz.wangdashe.top/gtyvverlid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtiafzuajd.html

[U115] JS：生成 UUID
来源：http://hz.svipenyu.cn/gtccxndlhz.html

crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtcxkknmwt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.fzhhl.top/gtnkumtrft.html

/** @param {string} name */ function f(name) {}
来源：http://hz.bjfxy.top/gtcakdtlxe.html

[U117] JS：单元测试
来源：http://hz.hywenlv.cn/gtvswsweav.html

npm i -D vitest;  npx vitest
来源：http://hz.birdmap.top/gtuehvicnh.html

[U118] JS：开发服务器
来源：http://hz.zycfv.cn/gtolhrgexh.html

npm i -D vite;  npx vite
来源：http://hz.jinghuilouyu.cn/gtofkmovlk.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtbgfkkfww.html

npx vite build
来源：http://hz.52xcode.cn/gtwfpbidwh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jiagoushi.top/gtwrjkwflm.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtawqnqqud.html

================================================================================
来源：http://hz.ehwqpu.com/gtfoppinrn.html

统计汇总
来源：http://hz.xuanzx.com/gthdcgoueg.html

================================================================================
来源：http://hz.yonumen.top/gtkgtdxaeq.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtmgmvcpkc.html

Python ......... 252
来源：http://hz.chenjidiqi.icu/gtredwuhsz.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtyyifrncx.html

JavaScript ..... 252
来源：http://hz.shanyushiyangtech.top/gtprbhxfxv.html

TypeScript ..... 212
来源：http://hz.tanke756.top/gtbcyxhvff.html

Java ........... 212
来源：http://hz.jqgfzy.top/gtxjxmtlej.html

Go ............. 212
来源：http://hz.52xcode.cn/gtwcelfsuh.html

Ruby ........... 212
来源：http://hz.ehwqpu.com/gtkfulxegi.html

C# ............. 212
来源：http://hz.ywan-chungtsiang.top/gtjzxnnnvu.html

C .............. 30
来源：http://hz.hysaishi.cn/gtuqajsjly.html

C++ ............ 30
来源：http://hz.hnqzz.top/gtnevsumfp.html

SQL ............ 90
来源：http://hz.hfpthk.cn/gtcrlowqfi.html

Bash ........... 80
来源：http://hz.gaohongyu789.top/gtnbkmjrrq.html

Kotlin ......... 15
来源：http://hz.feifeiyinyue.top/gtyjxhxicg.html

Swift .......... 15
来源：http://hz.redwolf501.top/gtlakecjbq.html

Lua ............ 10
来源：http://hz.tian-w.cn/gtkkayzzzu.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gthayuvsmi.html

Scala .......... 10
来源：http://hz.yj20258888.top/gtzkddrrds.html

------------------------------------
来源：http://hz.gogol.net.cn/gtfpnraetp.html

合计 ........... 2106 条
来源：http://hz.ydjk.org.cn/gtxsiwxzaj.html

按章节统计：
来源：http://hz.shzxlz.cn/gtaalhnabr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtdqqrwexk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gttmcyomwu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gthgvkcrcs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gthyqmbzpf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.birdmap.top/gtbwivjuei.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jyoumei.cn/gtxqkaolxt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtosifeafh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtmqrnscof.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtpknpytok.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtpkthktaw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtzpwucskn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtdeyeztpu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtenbvqfsg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gaohongyu789.top/gtkquhlxfc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.meibo888.top/gtwdizrees.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtechrbzfh.html

Q SQL 专题                              90
来源：http://hz.yangfankeji.com/gtwapowgsp.html

R Bash 专题                             80
来源：http://hz.jiagoushi.top/gtkqdrfafi.html

S C / C++ 专题                          60
来源：http://hz.gogol.net.cn/gtubpfacyc.html

T 其他语言补充                          60
来源：http://hz.jyoumei.cn/gttkmzdedm.html

U 高频实用片段                         120
来源：http://hz.yuxming.cn/gtmnhnkcdt.html

------------------------------------
来源：http://hz.zhixingplan.top/gtfjppohoy.html

合计                                  2106 条
来源：http://hz.snrcjt.cn/gtlmilxzrj.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtasjnoaly.html

使用提醒
来源：http://hz.yj202588.top/gtmswyolky.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtkgfqeclw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yonumen.top/gtuqccjsdw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xylfe.cn/gtgolovcgb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.daria6918.cn/gtcfpwaqgd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.wangshuangyany.cn/gthmkqlbae.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cheryme.top/gttixyafhk.html

—— 文件结束 ——
来源：http://hz.xuanzx.com/gtxamqorvr.html

================================================================================
来源：http://hz.yanxiufei.cn/gttduzekkx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zycfv.cn/gttuaxrlso.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigufen.top/gtyzzzdplv.html

================================================================================
来源：http://hz.havefunace.top/gtoixezgze.html

【收录内容】
来源：http://hz.nwbrower.top/gttxwxsgla.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hongshengwenyu.top/gtpkmrixfh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ehwqpu.com/gtqfjazdry.html

SQL · Bash · C · C++
来源：http://hz.chenjidiqi.icu/gtagqkhrge.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtcowduqqm.html

【使用说明】
来源：http://hz.hnqzz.top/gtlbikqrth.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.feifeiyinyue.top/gtpwseibdv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xziqi.cn/gtuuljgkvo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gtsepzwykg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cdnleiting.top/gtiitsvnug.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtnztcvcok.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ehwqpu.com/gtbylckdbg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gogol.net.cn/gtotqevzaa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ivvv.top/gtxkmbjsha.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.tianlin.xyz/gthjjvthif.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gtogcpxurb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gtelzsbsjz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ybcxt.top/gtpjqcwmzd.html

【文件统计】
来源：http://hz.yangfankeji.com/gtilrianxx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtcayhrrnc.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtwaacsena.html

目  录
来源：http://hz.0kj1m.cn/gtzynxpoak.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtvntcadzl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gtebzrllvx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtwaghdurt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtvusabrav.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhoulong.xyz/gtpnayjbrk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhijiandao.cn/gtkmqjdqph.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtbibfqkcz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtmkpmjsdp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.iojbl.cn/gtteltbfem.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtwxgcuieh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtaeayylqj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtppnadzut.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtniqnfodo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtelmeffau.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.52xcode.cn/gtvziiozlt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.tianlin.xyz/gtczavfwfp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtaactbzlr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhoulong.xyz/gteumcdvxj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xylfe.cn/gtweczbuql.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gtehitldnx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtzlogkqrt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtdzvcggxc.html

================================================================================
来源：http://hz.nanxuanxn.top/gthfoirnhy.html

A. 基础语法与类型
来源：http://hz.yonumen.top/gtittpprsn.html

================================================================================
来源：http://hz.tian-w.cn/gticphbeix.html

[A01] Hello World
来源：http://hz.jqgufenzy.top/gtcmlnndhs.html

Py:   print("Hello, World!")
来源：http://hz.aizwys.cn/gtmpvokuqf.html

PHP:  echo "Hello, World!";
来源：http://hz.xuanzx.com/gtijuzozfy.html

JS:   console.log("Hello, World!");
来源：http://hz.bjfxy.top/gtyglxqfxa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xingfuxueyuan.xyz/gtayjpsxaz.html

Java: System.out.println("Hello, World!");
来源：http://hz.cashguo.top/gtjexwwutt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gtlfofgzpx.html

Ruby: puts "Hello, World!"
来源：http://hz.yongpay.top/gttilzoxrh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.quarkkingdee.top/gtjbdkzila.html

[A02] 变量声明与赋值
来源：http://hz.sweek.top/gteykwhqud.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jlsjyb.cn/gttglpddkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.xziqi.cn/gtrcvvbixl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.316326.xyz/gtflznumea.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jlsjyb.cn/gtmzpsobpx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinyuanbaomall.cn/gtkhmudtvu.html

Go:   name := "Alex"; age := 20
来源：http://hz.bjfxy.top/gtpheeilnu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hammf.cn/gtbwtqgwjo.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yuanzhike.top/gtabhgwmem.html

[A03] 常量定义
来源：http://hz.aizwys.cn/gtagtazlsm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hfpthk.cn/gtbhoxrdww.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtuzfkhvnk.html

JS:   const PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtoihurgth.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtcrpjjmnv.html

Java: static final double PI = 3.14159;
来源：http://hz.yvedp.cn/gtiwxhfqhw.html

Go:   const PI = 3.14159
来源：http://hz.tianlin.xyz/gtxxcmgdpk.html

Ruby: PI = 3.14159
来源：http://hz.shanyushiyangkeji.top/gtseaxarii.html

C#:   const double PI = 3.14159;
来源：http://hz.tian-w.cn/gteichvwjg.html

[A04] 判断变量类型
来源：http://hz.jiagoushi.top/gtanullvht.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhaomingkeji.xyz/gtmnzpbrsf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jqgfzy.top/gtjwgqsqnf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.quarkkingdee.top/gtguzyiofk.html

TS:   typeof x; x instanceof Date
来源：http://hz.xingfuxueyuan.xyz/gtywxaeuio.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pengpengdd.cyou/gtdiexucix.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxinkj.top/gtotjoqfxa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jqgufenzy.top/gtqhkmycbj.html

C#:   x.GetType().Name; x is int
来源：http://hz.yvedp.cn/gtfwqdexlw.html

[A05] 整数除法与取模
来源：http://hz.yangfankeji.com/gtliqxmbyu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinqigufen.top/gtruhswwcz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.guowangkeji.top/gtmvogiuug.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhengqikj.top/gtrvdatmqt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tanke756.top/gtusfcmzrk.html

Java: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtgyguscjo.html

Go:   7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtdrrlujxz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtankmrycn.html

C#:   7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtqympiyef.html

[A06] 字符串转数字
来源：http://hz.ydjk.org.cn/gtlitfgrfq.html

Py:   int("42"); float("3.14")
来源：http://hz.9152youxi.cn/gtgvrgtcwt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ivvv.top/gtyndmaqse.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shzxlz.cn/gtwtxarlps.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.meibo888.top/gtdhdpoigw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhijiandao.cn/gtcplkbqhu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shanyushiyangtech.top/gtvcravsgt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhixingplan.top/gtozgkmtqg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.bjfxy.top/gtykkgpniv.html

[A07] 数字转字符串
来源：http://hz.xylfe.cn/gttqbdgmoh.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtcfpbyjit.html

PHP:  (string) 42; strval(42)
来源：http://hz.sxryk.cn/gtnymyyxwv.html

JS:   String(42); (42).toString()
来源：http://hz.chenlongwang.top/gtmzmtvdrg.html

TS:   String(42)
来源：http://hz.jqgufenzy.top/gtdfsgjzyz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhengqikj.top/gtxgdzekxt.html

Go:   strconv.Itoa(42)
来源：http://hz.xinyue.icu/gtbkabvgzk.html

Ruby: 42.to_s
来源：http://hz.yj20258.top/gtyneotjrx.html

C#:   42.ToString()
来源：http://hz.tanke756.top/gtzazdlzft.html

[A08] 取整与四舍五入
来源：http://hz.hywenlv.cn/gthaqvttow.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ehwqpu.com/gtxguozwos.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tanke756.top/gtzlrnskrw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.316326.xyz/gtxtaebgxu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hnxiangtu.top/gtotvzffdq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hammf.cn/gtsaafmdsy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.smart0.xyz/gtzdjzbkiw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.hammf.cn/gtihrgimfo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.chenzaomai.com/gtlrmpynbg.html

[A09] 绝对值与最大最小值
来源：http://hz.gotoacloud.top/gtsienwekl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ybcxt.top/gtzapnbpni.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtafinmygp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.aizwys.cn/gtjdazlrre.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.haohaochexian.top/gtubatuoas.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xylfe.cn/gtwouyjgvn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.daxiang520.top/gtcsxwmjhv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jinyuanbaomall.cn/gtgztnkkov.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hongshengwenyu.top/gtpwwbodwt.html

[A10] 生成随机数
来源：http://hz.meibo888.top/gtnaphhjjj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hfpthk.cn/gtawymnzum.html

PHP:  random_int(1, 100);
来源：http://hz.birdmap.top/gtdsmfcbbm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gaohongyu789.top/gtmzvisvtx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jyoumei.cn/gtachlosjh.html

Java: new Random().nextInt(100) + 1
来源：http://hz.sufxvd.cn/gtnsrueliy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xylfe.cn/gtpuoebzki.html

Ruby: rand(1..100)
来源：http://hz.jyoumei.cn/gtgqvjgdiu.html

C#:   new Random().Next(1, 101)
来源：http://hz.gogol.net.cn/gtnvykjkan.html

[A11] 条件表达式（三元）
来源：http://hz.yj20258888.top/gtxvxkeibu.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yongpay.top/gtystmaopc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtghhvofyn.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gtkaauictt.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gteszdaicd.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtcowliein.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.birdmap.top/gtyhtusksy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yangfankeji.com/gthogpnszb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.redwolf501.top/gtitkmohrw.html

[A12] 字符串插值 / 格式化
来源：http://hz.shangyingyoupin.top/gtzoouydqw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yueranfly.top/gtqsjxptnp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.andypj.xyz/gtgkzlxrsl.html

JS:   `Hello, ${name}!`
来源：http://hz.tian-w.cn/gtcfjfgyba.html

TS:   `Hello, ${name}!`
来源：http://hz.jinqigfzy.top/gtxpbfpgxq.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.gotoacloud.top/gtmeephwhp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hysaishi.cn/gthcxgauvr.html

Ruby: "Hello, #{name}!"
来源：http://hz.svipenyu.cn/gtasprwspd.html

C#:   $"Hello, {name}!"
来源：http://hz.jqgufenzy.top/gtharmcpgd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jqgfzy.top/gtiovwqwbw.html

Py:   "第一行\n第二行"
来源：http://hz.yj202588.top/gthquvyfve.html

PHP:  "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtsbvucxvc.html

JS:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtczifwipf.html

TS:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtthofpfzp.html

Java: "第一行\n第二行"
来源：http://hz.pycfn.com/gtssbkoyrq.html

Go:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtegqltmza.html

Ruby: "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtiwamshnw.html

C#:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtdafolthy.html

[A14] 注释写法
来源：http://hz.gogol.net.cn/gtxsvajeyv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.quarkkingdee.top/gtgudnqanz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtklunoypt.html

JS:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtoyraihxu.html


<!-- 参考信息 -->