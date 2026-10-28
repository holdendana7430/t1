代发 wailian999

[U93] JS：模板字符串
来源：http://hz.ehwqpu.com/gtqxqqomzn.html

`共 ${n} 条`
来源：http://hz.yongpay.top/gtktwqason.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtztsqhzbq.html

const double = x => x * 2;
来源：http://hz.pengpengdd.cyou/gtnkuzuley.html

[U95] JS：Promise 包装
来源：http://hz.sweek.top/gtdyhkhuxk.html

new Promise((resolve, reject) => {})
来源：http://hz.0kj1m.cn/gtmvisyztw.html

[U96] JS：async/await 与异常
来源：http://hz.ppjwa.cn/gtyrhquvik.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtpsixaaxb.html

[U97] JS：并发请求
来源：http://hz.mhx1999.top/gtfctdbpes.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtpypxantb.html

[U98] JS：fetch 带 JSON
来源：http://hz.nwbrower.top/gtfgytvfab.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxuanxn.top/gtwcxiuywg.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtugsjtajr.html

el.addEventListener("click", e => {})
来源：http://hz.jinyuanbaomall.cn/gtgtqkfqtv.html

[U100] JS：DOM 查询
来源：http://hz.jlsjyb.cn/gtqcsbmgcc.html

document.querySelector(".item")
来源：http://hz.iojbl.cn/gtzptgyagz.html

[U101] JS：classList 操作
来源：http://hz.ivvv.top/gtjcfymgph.html

el.classList.toggle("active")
来源：http://hz.cdnleiting.top/gtnzgfsdza.html

[U102] JS：本地存储
来源：http://hz.9152youxi.cn/gtgcsbdkki.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtcakuqhzx.html

[U103] JS：定时器
来源：http://hz.jinqigufen.top/gtukyddkst.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tian-w.cn/gtouvctfyb.html

[U104] JS：防抖
来源：http://hz.quarkkingdee.top/gthkoidxca.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtefwuytwi.html

[U105] JS：节流
来源：http://hz.zycfv.cn/gtjjfhtobg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cashguo.top/gtzpilzkwp.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtpoaegvpt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuetiantiany.cn/gtaadqopbn.html

[U107] JS：数字千分位
来源：http://hz.hfpthk.cn/gtiaoxfkih.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tian-w.cn/gtmhzjxwui.html

[U108] JS：随机整数
来源：http://hz.jiagoushi.top/gtbrvkvrak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnqzz.top/gtnicsvtll.html

[U109] JS：数组分组
来源：http://hz.jinqigufen.top/gtcessfnlv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtvzyjypxz.html

[U110] JS：数组分块
来源：http://hz.ywan-chungtsiang.top/gtizhrbncf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sufxvd.cn/gtabfarbdn.html

[U111] JS：对象转 Map
来源：http://hz.chenlongwang.top/gtcdigllpb.html

new Map(Object.entries(obj))
来源：http://hz.0kj1m.cn/gtkjzmrkfu.html

[U112] JS：字符串补位
来源：http://hz.9152youxi.cn/gtggqhnjbt.html

"7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtuvywkrlt.html

[U113] JS：正则替换全部
来源：http://hz.jyoumei.cn/gtzhyjbihe.html

s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtxyjxibwe.html

[U114] JS：JSON 深比较
来源：http://hz.pengpengdd.cyou/gtxcfnqshy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtmsurflwt.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gtyehwlmlw.html

crypto.randomUUID()
来源：http://hz.aizwys.cn/gtnxclhflk.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gteddzjfbv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sweek.top/gtpbvdhdau.html

[U117] JS：单元测试
来源：http://hz.jyoumei.cn/gtsnwhsojs.html

npm i -D vitest;  npx vitest
来源：http://hz.nwbrower.top/gtiumxmaxh.html

[U118] JS：开发服务器
来源：http://hz.cheryme.top/gtirjylqzi.html

npm i -D vite;  npx vite
来源：http://hz.sufxvd.cn/gtjbkfccwx.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtdvnmvnkk.html

npx vite build
来源：http://hz.ydjk.org.cn/gtggjpnhdq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.pengpengdd.cyou/gtmsbydnmu.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtbwlczwdh.html

================================================================================
来源：http://hz.sysykeji.top/gtwbocxfqn.html

统计汇总
来源：http://hz.guowangkeji.top/gtljnzgldv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcsrgkskb.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtctpyihkj.html

Python ......... 252
来源：http://hz.xingfuxueyuan.xyz/gtkajtquac.html

PHP ............ 252
来源：http://hz.aizwys.cn/gtoegwlaru.html

JavaScript ..... 252
来源：http://hz.bjfxy.top/gtauijynma.html

TypeScript ..... 212
来源：http://hz.hywenlv.cn/gteveskbyo.html

Java ........... 212
来源：http://hz.0kj1m.cn/gtbmmebkny.html

Go ............. 212
来源：http://hz.shanyushiyangkeji.top/gtbpyjtlfi.html

Ruby ........... 212
来源：http://hz.aibaodan.cn/gtmupkbrlb.html

C# ............. 212
来源：http://hz.xuanzx.com/gteecwtela.html

C .............. 30
来源：http://hz.cucudq.cn/gtyaydudhd.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtnfilyqyv.html

SQL ............ 90
来源：http://hz.birdmap.top/gtjnytcive.html

Bash ........... 80
来源：http://hz.jyoumei.cn/gtfcmxvzxg.html

Kotlin ......... 15
来源：http://hz.zhengqikj.top/gtedwbmuii.html

Swift .......... 15
来源：http://hz.ydzc1.top/gtgtjxvmij.html

Lua ............ 10
来源：http://hz.kuanghao11.cn/gtumkltpul.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gtmlyhrtkf.html

Scala .......... 10
来源：http://hz.jlsjyb.cn/gtkmaffhsi.html

------------------------------------
来源：http://hz.cashguo.top/gtooufzyam.html

合计 ........... 2106 条
来源：http://hz.smart0.xyz/gtwgfwngdb.html

按章节统计：
来源：http://hz.xuanzx.com/gtdkrwwbak.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtjvvpihqk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtrgiegijz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtiotbltdq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtsfgbxwkn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tanke756.top/gtfowtsgzu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sufxvd.cn/gtyfxancko.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtfkogsxbs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangkeji.top/gtglvccyaz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gthcknttla.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtrhwqwkdo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtuptvdmxg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gttikleqvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtridcbrnq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtnwcyivrg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinyuanbaomall.cn/gtprvhwjzx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtaubemffz.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtpyieosak.html

R Bash 专题                             80
来源：http://hz.redwolf501.top/gtrcxurzei.html

S C / C++ 专题                          60
来源：http://hz.cucudq.cn/gtjmihhlbu.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gtghhunnjx.html

U 高频实用片段                         120
来源：http://hz.tianlin.xyz/gthwfftgtd.html

------------------------------------
来源：http://hz.cucudq.cn/gtqwudpzck.html

合计                                  2106 条
来源：http://hz.chenjidiqi.icu/gtshohpajp.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtuvcxbkxo.html

使用提醒
来源：http://hz.tian-w.cn/gtlxcrrefo.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtvifgsqnm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ybcxt.top/gtqfcjpspx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.9152youxi.cn/gtoaljlrya.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.c1oappe.top/gtvknukufq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinghuilouyu.cn/gtymqdxpqq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhengqikj.top/gtthvcnkjo.html

—— 文件结束 ——
来源：http://hz.hywenlv.cn/gtlhtuuavp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqjysqzgx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.svipenyu.cn/gtmponkxkb.html

Common Programming Examples Cheat Book
来源：http://hz.cashguo.top/gtgucuzcgj.html

================================================================================
来源：http://hz.meibo888.top/gtjhkvlojo.html

【收录内容】
来源：http://hz.zhiwuduotai.top/gtxemabxio.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtbhvdbagn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.pengpengdd.cyou/gtymtwbyng.html

SQL · Bash · C · C++
来源：http://hz.aizwys.cn/gtgukagmij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.bjfxy.top/gtnuitmcxn.html

【使用说明】
来源：http://hz.yuanzhike.top/gtuocqxvzt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guannengcc.top/gtgwrtezbo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shanyushiyangtech.top/gtlgnadsob.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhengqikj.top/gtocotfsor.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hongshengwenyu.top/gtqrtovqsu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxinkj.top/gtjpddapmd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gthdckfkqs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.c1oappe.top/gthgdcniqw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.316326.xyz/gtnikpneup.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigfzy.top/gtykvnqmot.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yangfankeji.com/gtknkufcmw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jlsjyb.cn/gtmkjzszas.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.0kj1m.cn/gtsdbibbhd.html

【文件统计】
来源：http://hz.haohaochexian.top/gtruirqkgm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xuanzx.com/gtlftnnnjk.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtzfxdztfw.html

目  录
来源：http://hz.ivvv.top/gtlfvzpktr.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtcxjatjyq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenjidiqi.icu/gtnijgfbui.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hongshengwenyu.top/gtsfnqnlpd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gthprnuyln.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ehwqpu.com/gtcboeyrhv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhaomingkeji.xyz/gtvwjgqacn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtwyfgfbno.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.0kj1m.cn/gtwrgogmll.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cheryme.top/gthoygkasd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gthpelqwrn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gturjosktf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtlowlxsjq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtqszmszqy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtjqwceqwh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gtbozblarj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenjidiqi.icu/gtdybkdpds.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtiyhsyxlp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sxryk.cn/gtzwpskbov.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.vqdsnc.cn/gtldxpjlbg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj202588.top/gtfpygvoma.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtjtzeurig.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtgmdgfxlj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwzqvpagp.html

A. 基础语法与类型
来源：http://hz.smart0.xyz/gtmzvgtepq.html

================================================================================
来源：http://hz.gogol.net.cn/gtckeexvvm.html

[A01] Hello World
来源：http://hz.hongshengwenyu.top/gtsmwahtba.html

Py:   print("Hello, World!")
来源：http://hz.sufxvd.cn/gtivikudxa.html

PHP:  echo "Hello, World!";
来源：http://hz.svipenyu.cn/gtiidmrcpj.html

JS:   console.log("Hello, World!");
来源：http://hz.316326.xyz/gtblnfxlyj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinyuanbaomall.cn/gteefgmtdk.html

Java: System.out.println("Hello, World!");
来源：http://hz.shanyushiyangkeji.top/gtnzqaqsop.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj202588.top/gtdojinyyq.html

Ruby: puts "Hello, World!"
来源：http://hz.gotoacloud.top/gtdhphkoat.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.bjfxy.top/gtojkyqddk.html

[A02] 变量声明与赋值
来源：http://hz.aibaodan.cn/gtwhtjcelq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cucudq.cn/gtcomsjkdm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.c1oappe.top/gtlaglgeiv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.kuanghao11.cn/gtlqrssgep.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ywan-chungtsiang.top/gtbfoxchei.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ybcxt.top/gtzkqapkma.html

Go:   name := "Alex"; age := 20
来源：http://hz.ydjk.org.cn/gtdchsigrd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jiagoushi.top/gtmqdwkcmp.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yanxiufei.cn/gtozuixoor.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gttkycxjdm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hammf.cn/gtppjulvcy.html

PHP:  const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtpwbchmrr.html

JS:   const PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtiegixxit.html

TS:   const PI: number = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtkempicku.html

Java: static final double PI = 3.14159;
来源：http://hz.hnqzz.top/gtcsfcdwwh.html

Go:   const PI = 3.14159
来源：http://hz.andypj.xyz/gtwamutckc.html

Ruby: PI = 3.14159
来源：http://hz.pycfn.com/gtcywhqznb.html

C#:   const double PI = 3.14159;
来源：http://hz.cdnleiting.top/gtzftvruil.html

[A04] 判断变量类型
来源：http://hz.zdqjudy.top/gtrzbobqkg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jqgfzy.top/gtxsorhddj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.andypj.xyz/gtelbwgwqt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.dianchejie.cn/gtmjklpbze.html

TS:   typeof x; x instanceof Date
来源：http://hz.0kj1m.cn/gtewunjctd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.svipenyu.cn/gtmnpkdjad.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gthqmnkknk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhaomingkeji.xyz/gtvhpbacfr.html

C#:   x.GetType().Name; x is int
来源：http://hz.yuxming.cn/gtyairlofy.html

[A05] 整数除法与取模
来源：http://hz.jianghu66.top/gtzitimvee.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cucudq.cn/gtepdlptpe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.sufxvd.cn/gtipflimnu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guannengcc.top/gthgxncctr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daxiang520.top/gtjzkqwxfm.html

Java: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtobndsvaa.html

Go:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtvscswajy.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtthirlkix.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtsmdwgaxe.html

[A06] 字符串转数字
来源：http://hz.ydzc1.top/gthxxabgjj.html

Py:   int("42"); float("3.14")
来源：http://hz.hywenlv.cn/gtalfxacsm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jqgufenzy.top/gteijvbfxz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.9152youxi.cn/gtvitmvgmf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jyoumei.cn/gtjyczwnvf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yonumen.top/gtbosdniew.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jqgfzy.top/gtwdggjuff.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.fengsongda.top/gtvduzobgv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.gaohongyu789.top/gtnnbbglpe.html

[A07] 数字转字符串
来源：http://hz.hnxiangtu.top/gtuhtozbpn.html

Py:   str(42)
来源：http://hz.bjfxy.top/gtxmrccopk.html

PHP:  (string) 42; strval(42)
来源：http://hz.xingfuxueyuan.xyz/gtkfnpnpjl.html

JS:   String(42); (42).toString()
来源：http://hz.xinyue.icu/gtumnxjfkd.html

TS:   String(42)
来源：http://hz.nanxinkj.top/gtyypnffsg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.mhx1999.top/gtohimcojn.html

Go:   strconv.Itoa(42)
来源：http://hz.sweek.top/gtscsxbvoh.html

Ruby: 42.to_s
来源：http://hz.ppjwa.cn/gtmmqbwngr.html

C#:   42.ToString()
来源：http://hz.xylfe.cn/gtrwmqnpcf.html

[A08] 取整与四舍五入
来源：http://hz.gzhubu.top/gthzzyzwpi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gtlhifatrm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.0kj1m.cn/gtiwbnfvcg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinqigufen.top/gtweigpuhe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangtech.top/gtefnkndjf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.mhx1999.top/gtmteyhaxk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtebnczgmr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.meibo888.top/gtjfjrogen.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.quarkkingdee.top/gtbldhkqqc.html

[A09] 绝对值与最大最小值
来源：http://hz.jinghuilouyu.cn/gtyzgjnjha.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yonumen.top/gtjqmcaatj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenjidiqi.icu/gtmjcgkqef.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yuxming.cn/gtblodtkcx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.fengsongda.top/gtjiusubpl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yangfankeji.com/gtwzmdvrec.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhengqikj.top/gtnoagyhhw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.sxryk.cn/gtluhunoyf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.dashuyun.cn/gtlplskzuf.html

[A10] 生成随机数
来源：http://hz.xuanzx.com/gtcxkoexbd.html

Py:   import random; random.randint(1, 100)
来源：http://hz.haohaochexian.top/gtudqnuwkh.html

PHP:  random_int(1, 100);
来源：http://hz.daxiang520.top/gtjchsmwbu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.feifeiyinyue.top/gtxutlneko.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xuanzx.com/gtkzfmjlas.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gaohongyu789.top/gtmicihudz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.aizwys.cn/gtdmkclbvg.html

Ruby: rand(1..100)
来源：http://hz.316326.xyz/gtupairxlx.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuanzhike.top/gtsozsjmft.html

[A11] 条件表达式（三元）
来源：http://hz.shanyushiyangkeji.top/gtjasygkbp.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.fzhhl.top/gtohrrvvst.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yuxming.cn/gtkrkopbnh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtnyyktjul.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.dashuyun.cn/gtojnwlzlm.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.quarkkingdee.top/gtppmjfidm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jianghu66.top/gtirculivn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtvwotrmkl.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gthbrmeuzv.html

[A12] 字符串插值 / 格式化
来源：http://hz.cqqwz.cn/gtitwlwice.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jinghuilouyu.cn/gtmspyervg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.xylfe.cn/gthclulolo.html

JS:   `Hello, ${name}!`
来源：http://hz.yueranfly.top/gtbtctmjyk.html

TS:   `Hello, ${name}!`
来源：http://hz.mhx1999.top/gtnuyyfjnf.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.haohaochexian.top/gtmgnquelz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jiagoushi.top/gtabbeszbj.html

Ruby: "Hello, #{name}!"
来源：http://hz.jinghuilouyu.cn/gtvepdyzku.html

C#:   $"Hello, {name}!"
来源：http://hz.tian-w.cn/gtfpgxjlrn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hfpthk.cn/gtczcumhpz.html

Py:   "第一行\n第二行"
来源：http://hz.gogol.net.cn/gtgzeldqsz.html

PHP:  "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtivtdgarr.html

JS:   "第一行\n第二行"
来源：http://hz.yonumen.top/gtcpxsgmgc.html

TS:   "第一行\n第二行"
来源：http://hz.shzxlz.cn/gttvdodhgo.html

Java: "第一行\n第二行"
来源：http://hz.zycfv.cn/gtdjqzddiz.html

Go:   "第一行\n第二行"
来源：http://hz.havefunace.top/gttnajpyqm.html

Ruby: "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtvqvzsvam.html

C#:   "第一行\n第二行"
来源：http://hz.cheryme.top/gtuvcqqiuc.html

[A14] 注释写法
来源：http://hz.yanxiufei.cn/gtpizhayxh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hfpthk.cn/gtozbgcace.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jlsjyb.cn/gtcfxelrkp.html

JS:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtlhldcuqs.html

TS:   // 单行；/* 多行 */
来源：http://hz.dashuyun.cn/gttypxdfth.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yj202588.top/gtxfiqmjxg.html

Go:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gtsxymqxcb.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.tanke756.top/gtwemqbpfz.html

C#:   // 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtdnuwajpk.html

[A15] 空值判断与默认值
来源：http://hz.hnqzz.top/gtofxiysna.html

Py:   value = data or "默认值"
来源：http://hz.smart0.xyz/gtqavdqevu.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yongpay.top/gtxjmehhku.html

JS:   const value = data ?? "默认值";
来源：http://hz.haohaochexian.top/gtftnzqwhi.html

TS:   const value = data ?? "默认值";
来源：http://hz.jyoumei.cn/gtnflntndm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xziqi.cn/gtkyksbqid.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cqqwz.cn/gtbypuqhpw.html

Ruby: value = data || "默认值"
来源：http://hz.tian-w.cn/gtxnpglvbx.html

C#:   var value = data ?? "默认值";
来源：http://hz.nanxinkj.top/gtvvdgfczu.html

[A16] 真假值判断规则
来源：http://hz.sxryk.cn/gtzawryhil.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.gogol.net.cn/gtjspcmxhu.html


<!-- 参考信息 -->