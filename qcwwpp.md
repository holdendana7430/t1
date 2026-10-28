代发 wailian999

[U89] JS：数组去重
来源：http://hz.yj202588.top/gtvogfwckl.html

[...new Set(arr)]
来源：http://hz.sweek.top/gtshufpyzi.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangkeji.top/gtedzvbzkp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtjbwaszdf.html

[U91] JS：对象键值遍历
来源：http://hz.cashguo.top/gtigmjjcge.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.bjfxy.top/gtldkalqib.html

[U92] JS：深拷贝
来源：http://hz.daxiang520.top/gtxkorcart.html

structuredClone(obj)
来源：http://hz.sysykeji.top/gtvuoioaks.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtueqrmhkp.html

`共 ${n} 条`
来源：http://hz.dianchejie.cn/gtmvzppzqy.html

[U94] JS：箭头函数
来源：http://hz.cashguo.top/gtbvwkrwyz.html

const double = x => x * 2;
来源：http://hz.xinyue.icu/gtowdnvjur.html

[U95] JS：Promise 包装
来源：http://hz.daxiang520.top/gtuywwbfue.html

new Promise((resolve, reject) => {})
来源：http://hz.daria6918.cn/gtvbtattoi.html

[U96] JS：async/await 与异常
来源：http://hz.tian-w.cn/gtmlkozcwx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtlqcuhorc.html

[U97] JS：并发请求
来源：http://hz.tanke756.top/gtbuwwbspo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtdftbokso.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenlongwang.top/gtqggpcmtu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gzhubu.top/gtxzlxbbsu.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtodxysutn.html

el.addEventListener("click", e => {})
来源：http://hz.shuidangran.top/gtkmwrbrlp.html

[U100] JS：DOM 查询
来源：http://hz.316326.xyz/gtahwmbvqn.html

document.querySelector(".item")
来源：http://hz.hnqzz.top/gtrxlxqzba.html

[U101] JS：classList 操作
来源：http://hz.guannengcc.top/gtdhuosltv.html

el.classList.toggle("active")
来源：http://hz.shuidangran.top/gtapnirthx.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangtech.top/gtndjgjgvy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhixingplan.top/gttqiqzrxo.html

[U103] JS：定时器
来源：http://hz.jinyuanbaomall.cn/gtuwkccajb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xinyue.icu/gtwtdgageh.html

[U104] JS：防抖
来源：http://hz.gaohongyu789.top/gtrzywypop.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtevseoljr.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtrvdtulth.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhixingplan.top/gtzrnaunez.html

[U106] JS：日期格式化
来源：http://hz.sysykeji.top/gtjucmyexm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.haohaochexian.top/gtmuxfcfmc.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtrjkeealr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.redwolf501.top/gtvfappnlx.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtpzeqmtks.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hywenlv.cn/gtgnxdymdx.html

[U109] JS：数组分组
来源：http://hz.yuxming.cn/gtxenpybew.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtuahqsxdj.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtahbzyujk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj202588.top/gtdkscvzna.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtxclrdiok.html

new Map(Object.entries(obj))
来源：http://hz.yonumen.top/gtcjxtlnbq.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtfvnbwepp.html

"7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtdilfpuzi.html

[U113] JS：正则替换全部
来源：http://hz.jlsjyb.cn/gtiajmufky.html

s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtewmggnmc.html

[U114] JS：JSON 深比较
来源：http://hz.gzhubu.top/gtxchwjjvq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtoqaxlgtq.html

[U115] JS：生成 UUID
来源：http://hz.cheryme.top/gtnszfeioj.html

crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtxeupqkxv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhixingplan.top/gtfkfvjtxn.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinghuilouyu.cn/gtqgiulmju.html

[U117] JS：单元测试
来源：http://hz.wangshuangyany.cn/gtozfpvikl.html

npm i -D vitest;  npx vitest
来源：http://hz.xinyue.icu/gtlzogxvpc.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtjmmhzmtv.html

npm i -D vite;  npx vite
来源：http://hz.tian-w.cn/gthabisshc.html

[U119] JS：生产构建
来源：http://hz.andypj.xyz/gtlkkfasci.html

npx vite build
来源：http://hz.redwolf501.top/gtnaaffsri.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhijiandao.cn/gtcmidsqwp.html

import.meta.env.VITE_API_URL
来源：http://hz.316326.xyz/gtslsiulvk.html

================================================================================
来源：http://hz.iojbl.cn/gtpatdnosv.html

统计汇总
来源：http://hz.316326.xyz/gtoquvqapd.html

================================================================================
来源：http://hz.yvedp.cn/gttqfvmzoy.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtdxelrobo.html

Python ......... 252
来源：http://hz.yuxming.cn/gtzyljopbl.html

PHP ............ 252
来源：http://hz.yonumen.top/gtymdqclbh.html

JavaScript ..... 252
来源：http://hz.hongshengwenyu.top/gtfxxvbicr.html

TypeScript ..... 212
来源：http://hz.chenlongwang.top/gtszzfvzpa.html

Java ........... 212
来源：http://hz.nanxinkj.top/gtkydeavxn.html

Go ............. 212
来源：http://hz.hywenlv.cn/gtvqzyneeh.html

Ruby ........... 212
来源：http://hz.snrcjt.cn/gtjvjodlre.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtuizxpoet.html

C .............. 30
来源：http://hz.quarkkingdee.top/gtcsrnqshb.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtrjcoaavk.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtkaffgnip.html

Bash ........... 80
来源：http://hz.iojbl.cn/gtmrjuspku.html

Kotlin ......... 15
来源：http://hz.52xcode.cn/gtqsmyjvwh.html

Swift .......... 15
来源：http://hz.nanxuanxn.top/gtnobtamvg.html

Lua ............ 10
来源：http://hz.nanxuanxn.top/gtksvpxhdz.html

Perl ........... 10
来源：http://hz.birdmap.top/gtdgbpqiai.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtihcuojuq.html

------------------------------------
来源：http://hz.hywenlv.cn/gthaigamni.html

合计 ........... 2106 条
来源：http://hz.gzhubu.top/gtnfpuimle.html

按章节统计：
来源：http://hz.quarkkingdee.top/gtbehwftgp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gtgffqvthg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtrpvvmpgq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtakhikvbp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yonumen.top/gtzrzltshi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinghuilouyu.cn/gtzkchszas.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtsxbfylzq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtdgbsjrkw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtnhvsqiep.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gthqbnfiwb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jianghu66.top/gtbqgxlsyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtpbiemdeh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtapafiidy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtqvrwferz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtjrbazmqf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yongpay.top/gtsapttawz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gttqiypkkl.html

Q SQL 专题                              90
来源：http://hz.yvedp.cn/gteubitwpa.html

R Bash 专题                             80
来源：http://hz.yonumen.top/gtgxxdpppx.html

S C / C++ 专题                          60
来源：http://hz.pengpengdd.cyou/gtygfihsgs.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gtnwwbixla.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtszpnqyha.html

------------------------------------
来源：http://hz.ehwqpu.com/gtbygrnwme.html

合计                                  2106 条
来源：http://hz.nanxinkj.top/gtcevwvmxq.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtatoihvoq.html

使用提醒
来源：http://hz.redwolf501.top/gtdigznqii.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtndcywvdf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.chenlongwang.top/gtiixrvuhn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.dianchejie.cn/gtxdbwncqd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.bjfxy.top/gtlshoajow.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gotoacloud.top/gtvvgzinow.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hnxiangtu.top/gtvsqubgfq.html

—— 文件结束 ——
来源：http://hz.smart0.xyz/gthgtzmopd.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcnxicjdo.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shanyushiyangkeji.top/gtahjsdszl.html

Common Programming Examples Cheat Book
来源：http://hz.daxiang520.top/gthkfgatlr.html

================================================================================
来源：http://hz.0kj1m.cn/gtylvhjmdn.html

【收录内容】
来源：http://hz.hysaishi.cn/gtgwijyzcl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pycfn.com/gtiopnwgif.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gotoacloud.top/gtfpfbosyu.html

SQL · Bash · C · C++
来源：http://hz.hnqzz.top/gteinjubwq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.tian-w.cn/gtywzgtndh.html

【使用说明】
来源：http://hz.guannengcc.top/gtquyvadvo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cheryme.top/gttdjlrzpu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.bjfxy.top/gtbhbiqrju.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cucudq.cn/gtdhvrkoph.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shuidangran.top/gtlvgluqdj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yvedp.cn/gttzudogcd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gzhubu.top/gtllqeonof.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dianchejie.cn/gtqzdqgjie.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.bjfxy.top/gtaojujfdp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxuanxn.top/gtstrlfqpw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yongpay.top/gtcarjuxkr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gaohongyu789.top/gthoivhada.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daxiang520.top/gtilnuhndr.html

【文件统计】
来源：http://hz.wangdashe.top/gtqnoqvmul.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gtccgnvcwy.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtguvsfyzw.html

目  录
来源：http://hz.birdmap.top/gtrkhholxq.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtuylzxayi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtzuwfkryd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yuxming.cn/gtnwkbnopt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtlbizhndx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtobhlwhyw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shanyushiyangtech.top/gtdkxvneuu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.daria6918.cn/gtgqzvrlnt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhoulong.xyz/gtopuyolko.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.andypj.xyz/gtydhlkefy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtfiyhnedn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtpkdnokxm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtxmfewgpf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtmwprmpmx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtzkwoyyqq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangdashe.top/gtlnlxekqg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhengqikj.top/gtjfywzumf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtjfmncskm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtgsmlfifk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.quarkkingdee.top/gtixalcnng.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.fzhhl.top/gtgzotqqup.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtuccdirfx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtolrgjhpy.html

================================================================================
来源：http://hz.hammf.cn/gtdotbqmar.html

A. 基础语法与类型
来源：http://hz.zhaomingkeji.xyz/gtdhtqsano.html

================================================================================
来源：http://hz.yuxming.cn/gtjfvroqjn.html

[A01] Hello World
来源：http://hz.jqgufenzy.top/gtepaubcaq.html

Py:   print("Hello, World!")
来源：http://hz.yonumen.top/gtohyznapi.html

PHP:  echo "Hello, World!";
来源：http://hz.yanxiufei.cn/gthodobsku.html

JS:   console.log("Hello, World!");
来源：http://hz.jqgfzy.top/gtiezjfnyz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.aibaodan.cn/gtuckqvaal.html

Java: System.out.println("Hello, World!");
来源：http://hz.cdnleiting.top/gtsbnhwfbp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.fzhhl.top/gthpmufhcc.html

Ruby: puts "Hello, World!"
来源：http://hz.smart0.xyz/gtbnfombae.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.redwolf501.top/gtlmyfywmv.html

[A02] 变量声明与赋值
来源：http://hz.gotoacloud.top/gtdbafxgle.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.wangdashe.top/gttitaurxx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtctksfgoy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.fengsongda.top/gtqxaicgla.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jinqigufen.top/gtvgqqcxdh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtxbsrjapl.html

Go:   name := "Alex"; age := 20
来源：http://hz.9152youxi.cn/gtkqgkwdbs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shangyingyoupin.top/gtglhwvjcp.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.wangshuangyany.cn/gtxhqkqubc.html

[A03] 常量定义
来源：http://hz.hammf.cn/gtfyncswxu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxinkj.top/gtebeyksdb.html

PHP:  const PI = 3.14159;
来源：http://hz.daxiang520.top/gtroukbdeo.html

JS:   const PI = 3.14159;
来源：http://hz.jianghu66.top/gtapyzimtd.html

TS:   const PI: number = 3.14159;
来源：http://hz.dashuyun.cn/gthebpokro.html

Java: static final double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtajnxrzvo.html

Go:   const PI = 3.14159
来源：http://hz.fengsongda.top/gtrzoklfny.html

Ruby: PI = 3.14159
来源：http://hz.havefunace.top/gtkbjonifo.html

C#:   const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtxnwjbric.html

[A04] 判断变量类型
来源：http://hz.shangyingyoupin.top/gtsngzvvwn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yangfankeji.com/gtutcprzhx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.316326.xyz/gtekbqxdtb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yj20258.top/gtnmmvrgtp.html

TS:   typeof x; x instanceof Date
来源：http://hz.yuxming.cn/gtsebmrpiv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ywan-chungtsiang.top/gtqigxlsah.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cheryme.top/gttcbszrtf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sweek.top/gtqhjngazv.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtshurjdcu.html

[A05] 整数除法与取模
来源：http://hz.yuxming.cn/gtoorsjuwk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ehwqpu.com/gthlxyrnlk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cashguo.top/gtuwhqivlh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtbqutipue.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.316326.xyz/gtglsnrcin.html

Java: 7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtuhsepubu.html

Go:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtceenguhs.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gthuktqrkh.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuxming.cn/gtoshaipni.html

[A06] 字符串转数字
来源：http://hz.xylfe.cn/gtziuyfova.html

Py:   int("42"); float("3.14")
来源：http://hz.zhixingplan.top/gticamyjhg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yj20258888.top/gtfnpaqhbz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ivvv.top/gtvqjpnuok.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hysaishi.cn/gttcqdculn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yonumen.top/gtojohutgh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ydzc1.top/gtchaukbwc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.pycfn.com/gtyqiddcdk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yueranfly.top/gtimvdzcxz.html

[A07] 数字转字符串
来源：http://hz.zhijiandao.cn/gtkkpmxfms.html

Py:   str(42)
来源：http://hz.hysaishi.cn/gtzvdnmqoq.html

PHP:  (string) 42; strval(42)
来源：http://hz.ybcxt.top/gtvwzocpbj.html

JS:   String(42); (42).toString()
来源：http://hz.mhx1999.top/gtyxbbhcsw.html

TS:   String(42)
来源：http://hz.jinqigufen.top/gtrluokacv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yj202588.top/gtzljesauq.html

Go:   strconv.Itoa(42)
来源：http://hz.yj20258.top/gtaoqxcwnk.html

Ruby: 42.to_s
来源：http://hz.nwbrower.top/gtsqyxyhbk.html

C#:   42.ToString()
来源：http://hz.daria6918.cn/gtlbctvdja.html

[A08] 取整与四舍五入
来源：http://hz.zhongyouzk.top/gtryonuhsh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cheryme.top/gtlycdulbn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dashuyun.cn/gtgcgcrjrt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hfpthk.cn/gtsjpewszu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xylfe.cn/gtidfowowe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cucudq.cn/gticsidwtg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhengqikj.top/gtcgnpwgay.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenlongwang.top/gtzmzjingz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yonumen.top/gtzlcnydwd.html

[A09] 绝对值与最大最小值
来源：http://hz.aizwys.cn/gtgrjzoyid.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cqqwz.cn/gtkpomelyu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guannengcc.top/gtjikgaxsb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ivvv.top/gtphpwqtui.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nwbrower.top/gtmfcylqts.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hywenlv.cn/gtlhvuowql.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.snrcjt.cn/gtocivmskb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shzxlz.cn/gtpcbfctbw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.andypj.xyz/gtiiwowybr.html

[A10] 生成随机数
来源：http://hz.jinqigufen.top/gtdptxrdxf.html

Py:   import random; random.randint(1, 100)
来源：http://hz.chenjidiqi.icu/gttqmmslxc.html

PHP:  random_int(1, 100);
来源：http://hz.jianghu66.top/gtrlongtlt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.mhx1999.top/gtwuntijjc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ybcxt.top/gtacgnzscw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.fzhhl.top/gtiimiyivi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinyuanbaomall.cn/gtxoxjetxx.html

Ruby: rand(1..100)
来源：http://hz.xinyue.icu/gtrvtobvzc.html

C#:   new Random().Next(1, 101)
来源：http://hz.dianchejie.cn/gtczksamgc.html

[A11] 条件表达式（三元）
来源：http://hz.chenzaomai.com/gtfevkyyxg.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.nanxinkj.top/gtolgqtfiy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gtcynsiulj.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gtivqemwpf.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtnxyihysd.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ivvv.top/gtwfqfaaqg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.cdnleiting.top/gtizthnvan.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtawtbfeav.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtepxsrhtv.html

[A12] 字符串插值 / 格式化
来源：http://hz.nanxinkj.top/gtdacmlona.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.fengsongda.top/gtbbvfvjec.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ppjwa.cn/gtjfqtahlc.html

JS:   `Hello, ${name}!`
来源：http://hz.sufxvd.cn/gtwvkbjucn.html

TS:   `Hello, ${name}!`
来源：http://hz.guannengcc.top/gtrvajtqjn.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ydjk.org.cn/gtfkdpniuk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.snrcjt.cn/gtqcntqxrl.html

Ruby: "Hello, #{name}!"
来源：http://hz.gotoacloud.top/gtpfyxmbht.html

C#:   $"Hello, {name}!"
来源：http://hz.0kj1m.cn/gtwmlzktve.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hysaishi.cn/gtjycvqgdp.html

Py:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtwseylzgb.html

PHP:  "第一行\n第二行"
来源：http://hz.svipenyu.cn/gtlfpwytcq.html

JS:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gthmjgzmch.html

TS:   "第一行\n第二行"
来源：http://hz.xuetiantiany.cn/gtpqxagonc.html

Java: "第一行\n第二行"
来源：http://hz.52xcode.cn/gtwixykyth.html

Go:   "第一行\n第二行"
来源：http://hz.sweek.top/gtmpfhhxhs.html

Ruby: "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gtyjxybzja.html

C#:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtyeeauinv.html

[A14] 注释写法
来源：http://hz.yonumen.top/gtxpxesarp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.wangshuangyany.cn/gtzqpjgaql.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jqgufenzy.top/gtfotdrpdl.html

JS:   // 单行；/* 多行 */
来源：http://hz.jqgfzy.top/gtbgjjkces.html

TS:   // 单行；/* 多行 */
来源：http://hz.meibo888.top/gttfbzjfqp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.redwolf501.top/gtigusacyb.html

Go:   // 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtzfingdba.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.tanke756.top/gtljfudxfj.html

C#:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtvcrctydk.html

[A15] 空值判断与默认值
来源：http://hz.yj20258.top/gtjdvatlsl.html

Py:   value = data or "默认值"
来源：http://hz.redwolf501.top/gtnrdbfufy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.nanxuanxn.top/gturithohh.html


<!-- 参考信息 -->