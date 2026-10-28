代发 wailian999

[U93] JS：模板字符串
来源：http://hz.feifeiyinyue.top/gtgboptjas.html

`共 ${n} 条`
来源：http://hz.9152youxi.cn/gtrajbfkla.html

[U94] JS：箭头函数
来源：http://hz.ydzc1.top/gtwfgxfxuz.html

const double = x => x * 2;
来源：http://hz.guowangkeji.top/gtpylzifbw.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtggjsgapu.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gthadrvpxf.html

[U96] JS：async/await 与异常
来源：http://hz.shuidangran.top/gtqxdyeseq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtcsnsegro.html

[U97] JS：并发请求
来源：http://hz.nwbrower.top/gtlptpblbc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtawwsztxk.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhaomingkeji.xyz/gtbrtsbbtr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxuanxn.top/gtbcogwynb.html

[U99] JS：事件监听
来源：http://hz.jqgfzy.top/gtrluxxmzn.html

el.addEventListener("click", e => {})
来源：http://hz.ydzc1.top/gttsmquuyb.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtzkljdtpe.html

document.querySelector(".item")
来源：http://hz.ywan-chungtsiang.top/gtecxjsfqm.html

[U101] JS：classList 操作
来源：http://hz.xuanzx.com/gtdkrczfnq.html

el.classList.toggle("active")
来源：http://hz.daria6918.cn/gtlivtxqib.html

[U102] JS：本地存储
来源：http://hz.hammf.cn/gtimqpopiv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.daria6918.cn/gthacbleij.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gtgbufdmoi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhengqikj.top/gttohipjax.html

[U104] JS：防抖
来源：http://hz.52xcode.cn/gtpkevjjpt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtpldkxfhe.html

[U105] JS：节流
来源：http://hz.sysykeji.top/gtwzdyewcg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangshuangyany.cn/gtxlnyuzlp.html

[U106] JS：日期格式化
来源：http://hz.wangshuangyany.cn/gtohpphxeu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.svipenyu.cn/gtgcztzmly.html

[U107] JS：数字千分位
来源：http://hz.nwbrower.top/gtvsnvehst.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigufen.top/gtyihqasid.html

[U108] JS：随机整数
来源：http://hz.jlsjyb.cn/gtokrojgwv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.c1oappe.top/gthybtazld.html

[U109] JS：数组分组
来源：http://hz.haohaochexian.top/gtqvafgwyi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtrbsjajmf.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtpxymremk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinyuanbaomall.cn/gtovfqjohi.html

[U111] JS：对象转 Map
来源：http://hz.mhx1999.top/gtmsazowoq.html

new Map(Object.entries(obj))
来源：http://hz.ydzc1.top/gtmgfordlf.html

[U112] JS：字符串补位
来源：http://hz.iojbl.cn/gtogstimhu.html

"7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtizfcblhh.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gthdfcpvnr.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gthdakjqly.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtegywhmpv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtbxkwxkhy.html

[U115] JS：生成 UUID
来源：http://hz.cqqwz.cn/gtjetyfiar.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gthitxjlub.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnxiangtu.top/gtomqegbmg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtdntfcnbo.html

[U117] JS：单元测试
来源：http://hz.smart0.xyz/gtqpzqaoxe.html

npm i -D vitest;  npx vitest
来源：http://hz.wangdashe.top/gtxznbveok.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtcgopwctm.html

npm i -D vite;  npx vite
来源：http://hz.sxryk.cn/gtndtpuclp.html

[U119] JS：生产构建
来源：http://hz.sysykeji.top/gthawltdsk.html

npx vite build
来源：http://hz.guowangkeji.top/gtjfihclki.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgfzy.top/gtvxdgdeol.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gttesiloes.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtowaayeju.html

统计汇总
来源：http://hz.zhiwuduotai.top/gtdkkvmusv.html

================================================================================
来源：http://hz.snrcjt.cn/gtiepplkgn.html

按语言统计（条）：
来源：http://hz.wangshuangyany.cn/gtgjvdenux.html

Python ......... 252
来源：http://hz.gotoacloud.top/gtmrkddqre.html

PHP ............ 252
来源：http://hz.cucudq.cn/gtxwqhgskc.html

JavaScript ..... 252
来源：http://hz.jiagoushi.top/gtiwtoyasx.html

TypeScript ..... 212
来源：http://hz.yuanzhike.top/gtiqbndhxx.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtgsbhlncy.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gtdmxsagqq.html

Ruby ........... 212
来源：http://hz.xylfe.cn/gtrwnanhku.html

C# ............. 212
来源：http://hz.sxryk.cn/gtxrtfcviw.html

C .............. 30
来源：http://hz.0kj1m.cn/gtgtehjabq.html

C++ ............ 30
来源：http://hz.yuanzhike.top/gthlopyimk.html

SQL ............ 90
来源：http://hz.yvedp.cn/gttjqvpkpm.html

Bash ........... 80
来源：http://hz.jqgufenzy.top/gtnpkyefzj.html

Kotlin ......... 15
来源：http://hz.chenzaomai.com/gtqflugwnp.html

Swift .......... 15
来源：http://hz.sufxvd.cn/gtixgtnlrc.html

Lua ............ 10
来源：http://hz.0kj1m.cn/gtfeehcxpw.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtsmsibiop.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtjnzorahp.html

------------------------------------
来源：http://hz.mhx1999.top/gtojjszzwz.html

合计 ........... 2106 条
来源：http://hz.hongshengwenyu.top/gttmtbvrvy.html

按章节统计：
来源：http://hz.ppjwa.cn/gtcqhghxgd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gtslximmyy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtwflsxucb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtsasklkur.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtduuxiqmp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jqgfzy.top/gtwdfrfddx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtyskwhyug.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gtlchavakt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtlhykoicy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtczfjplnd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenjidiqi.icu/gtlsqvktzm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtpdpsyqso.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtxlmjbjtb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtgqirouvw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtnpahhjtj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.aizwys.cn/gtdrmkcrbz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtffxevqqp.html

Q SQL 专题                              90
来源：http://hz.nanxuanxn.top/gtrjplnqim.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtqmghpgnt.html

S C / C++ 专题                          60
来源：http://hz.hywenlv.cn/gtyobxawbh.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtonabwfzl.html

U 高频实用片段                         120
来源：http://hz.aizwys.cn/gtzeqynmrp.html

------------------------------------
来源：http://hz.hywenlv.cn/gtiuupesnu.html

合计                                  2106 条
来源：http://hz.yangfankeji.com/gtndlyteep.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gttvrnscot.html

使用提醒
来源：http://hz.hnqzz.top/gtiwpybndu.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtpnpafeeo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.0kj1m.cn/gtishdnhfg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtevaoinyj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.9152youxi.cn/gtapgseqjx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.aibaodan.cn/gtkuxllpsp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cashguo.top/gtkirtktdr.html

—— 文件结束 ——
来源：http://hz.jinqigfzy.top/gtdzqytlaf.html

================================================================================
来源：http://hz.ydzc1.top/gtuktdcqmr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhaomingkeji.xyz/gtlwdsvrgp.html

Common Programming Examples Cheat Book
来源：http://hz.mhx1999.top/gtlexiubog.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwnuaofck.html

【收录内容】
来源：http://hz.yueranfly.top/gtpegwebfm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xingfuxueyuan.xyz/gtofiqjfrk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xuetiantiany.cn/gtelixzust.html

SQL · Bash · C · C++
来源：http://hz.andypj.xyz/gtnopyughx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.pycfn.com/gtlpxzbvph.html

【使用说明】
来源：http://hz.316326.xyz/gtrshcacdy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shangyingyoupin.top/gtbekxiajf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.fzhhl.top/gthubmiyyd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ehwqpu.com/gtokmbaklt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.smart0.xyz/gtiqpebwjd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hnxiangtu.top/gtnhryjzxc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ehwqpu.com/gtosxtiecs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangshuangyany.cn/gtfculgwnd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtprnttuzq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.vqdsnc.cn/gtwggswlwv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tian-w.cn/gtlmctmqjf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhengqikj.top/gtjptqhdyr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aibaodan.cn/gtujmqmrjf.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gteicvhsqk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.chenjidiqi.icu/gtcviwbayg.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtxpcdbctp.html

目  录
来源：http://hz.vqdsnc.cn/gtupupjkuc.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtxjurktnp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtbdbgjklk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ehwqpu.com/gtuyihwvss.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gtgkgmjqai.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtbfqduwbj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tanke756.top/gteyqpidtf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.316326.xyz/gtmoaloisq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtcwkinlfd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhixingplan.top/gtlwesrlsv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtwclnwjta.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.316326.xyz/gtwkqobvqo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtotmnigzb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtxblctbuv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtrndbrask.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tanke756.top/gtogpjpmjd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.haohaochexian.top/gtaruakouh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtdoxputgh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangdashe.top/gtujtiodqb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shuidangran.top/gtktkxnhxk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dashuyun.cn/gtgpafxguq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtglfdqiqp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtsdcuuozp.html

================================================================================
来源：http://hz.yangfankeji.com/gtsqfkflub.html

A. 基础语法与类型
来源：http://hz.hysaishi.cn/gtvfkbgiei.html

================================================================================
来源：http://hz.yj202588.top/gtlgnxudaj.html

[A01] Hello World
来源：http://hz.zycfv.cn/gttibabojg.html

Py:   print("Hello, World!")
来源：http://hz.redwolf501.top/gtlchnaaut.html

PHP:  echo "Hello, World!";
来源：http://hz.quarkkingdee.top/gtlczurhvq.html

JS:   console.log("Hello, World!");
来源：http://hz.xinyue.icu/gtklbvufns.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cucudq.cn/gtqqnqzjpu.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gtiwatexsr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.daria6918.cn/gtrunadkew.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtqekaxcyg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.svipenyu.cn/gtzbqumgbh.html

[A02] 变量声明与赋值
来源：http://hz.yueranfly.top/gtactxkovs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xinyue.icu/gtbxutqbpz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nwbrower.top/gtmaccsiuk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.daria6918.cn/gtlpfglptl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yj20258.top/gtxhgojewx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.mhx1999.top/gtdokigdgq.html

Go:   name := "Alex"; age := 20
来源：http://hz.gotoacloud.top/gttacvuuwy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ydzc1.top/gtxckcfhsl.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtjcujaggg.html

[A03] 常量定义
来源：http://hz.redwolf501.top/gtrlsqnpdy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.wangdashe.top/gtasqukyxl.html

PHP:  const PI = 3.14159;
来源：http://hz.gzhubu.top/gtddoddgrx.html

JS:   const PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtavszpisx.html

TS:   const PI: number = 3.14159;
来源：http://hz.gaohongyu789.top/gtbwphepjt.html

Java: static final double PI = 3.14159;
来源：http://hz.aizwys.cn/gtuvpflmht.html

Go:   const PI = 3.14159
来源：http://hz.sxryk.cn/gtqkfuwrif.html

Ruby: PI = 3.14159
来源：http://hz.gaohongyu789.top/gtegzavcib.html

C#:   const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtlrsbkfeo.html

[A04] 判断变量类型
来源：http://hz.gaohongyu789.top/gtgkhdtfce.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.andypj.xyz/gtfqlzkbag.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.meibo888.top/gtvxhxfzio.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ydjk.org.cn/gtzlilapoi.html

TS:   typeof x; x instanceof Date
来源：http://hz.dianchejie.cn/gtqhkoscgp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.mhx1999.top/gtkkfroghe.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ehwqpu.com/gtzqfdkvsm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ybcxt.top/gtqzxnsngd.html

C#:   x.GetType().Name; x is int
来源：http://hz.pycfn.com/gtmoojijxo.html

[A05] 整数除法与取模
来源：http://hz.cdnleiting.top/gtqvwckqme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangtech.top/gttedmzrqc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.havefunace.top/gtwrznvknq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ivvv.top/gtwktbcegu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtlcsipcfo.html

Java: 7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtaghwxndb.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtfuemryvs.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtwzvchang.html

C#:   7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtpgwajeul.html

[A06] 字符串转数字
来源：http://hz.shangyingyoupin.top/gtfkqrdzvp.html

Py:   int("42"); float("3.14")
来源：http://hz.guowangkeji.top/gtqjqrnyoi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gotoacloud.top/gtmxfjftde.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtbvjpduub.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.9152youxi.cn/gtjhlfvwex.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cheryme.top/gtxxmyfayo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhoulong.xyz/gtouvznlco.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhiwuduotai.top/gtiwdvabqu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.52xcode.cn/gttvyxkotb.html

[A07] 数字转字符串
来源：http://hz.ivvv.top/gteacegsem.html

Py:   str(42)
来源：http://hz.sxryk.cn/gtsagmzowz.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhoulong.xyz/gtwitoclpc.html

JS:   String(42); (42).toString()
来源：http://hz.fengsongda.top/gtgqpetsry.html

TS:   String(42)
来源：http://hz.jianghu66.top/gtvklstuol.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.mhx1999.top/gtjydrempo.html

Go:   strconv.Itoa(42)
来源：http://hz.jinghuilouyu.cn/gtyecnpcwi.html

Ruby: 42.to_s
来源：http://hz.haohaochexian.top/gtdlfcyegr.html

C#:   42.ToString()
来源：http://hz.yuanzhike.top/gthityfmsh.html

[A08] 取整与四舍五入
来源：http://hz.zhijiandao.cn/gtbhkxmjxn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.daria6918.cn/gtemxvnosn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.snrcjt.cn/gthjuzicqh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.haohaochexian.top/gtupnvedeg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.meibo888.top/gtyswbznjc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yanxiufei.cn/gtncctiddd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtvhmdfvhg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.9152youxi.cn/gtiijixqxx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hfpthk.cn/gtkyegrhzs.html

[A09] 绝对值与最大最小值
来源：http://hz.zhoulong.xyz/gtuovewjgx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtjrvwcldj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinghuilouyu.cn/gtuwyftuqa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nanxuanxn.top/gttoosfeau.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtznhmczbq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.wangdashe.top/gtkkbkkdqt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.kuanghao11.cn/gtcsewomus.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jqgfzy.top/gtsxpfoohb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenlongwang.top/gtblmdcyvm.html

[A10] 生成随机数
来源：http://hz.kuanghao11.cn/gtpettmffj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.0kj1m.cn/gtrnrqdnvt.html

PHP:  random_int(1, 100);
来源：http://hz.cdnleiting.top/gtwccxewip.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sufxvd.cn/gtgcopmtde.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zdqjudy.top/gtkmgfwqyw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.sweek.top/gtfonykket.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hnqzz.top/gtxzwusdbh.html

Ruby: rand(1..100)
来源：http://hz.svipenyu.cn/gtiwsoroct.html

C#:   new Random().Next(1, 101)
来源：http://hz.xylfe.cn/gttjndvxkh.html

[A11] 条件表达式（三元）
来源：http://hz.quarkkingdee.top/gtvtgiahqn.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.52xcode.cn/gtiiwntbkz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtpsajrcrm.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.dashuyun.cn/gtrnmrukji.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtlbedljmu.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yuanzhike.top/gtahvwbvoi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jianghu66.top/gtrhjgmevv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhoulong.xyz/gtkvjanhyp.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtdfgaqvod.html

[A12] 字符串插值 / 格式化
来源：http://hz.ybcxt.top/gtdlsuldgv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shuidangran.top/gtnchjkafm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yonumen.top/gtfufjlkxm.html

JS:   `Hello, ${name}!`
来源：http://hz.ybcxt.top/gtzezasozg.html

TS:   `Hello, ${name}!`
来源：http://hz.feifeiyinyue.top/gtrzzjmxga.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.chenzaomai.com/gtvbodwygf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gogol.net.cn/gtfspbugmy.html

Ruby: "Hello, #{name}!"
来源：http://hz.gogol.net.cn/gtmbwmcjvr.html

C#:   $"Hello, {name}!"
来源：http://hz.andypj.xyz/gtbrqkhikx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.feifeiyinyue.top/gtmciwelvy.html

Py:   "第一行\n第二行"
来源：http://hz.feifeiyinyue.top/gtdkgvditk.html

PHP:  "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtfjqjoopv.html

JS:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtbfhntoau.html

TS:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtdssdpqhy.html

Java: "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtydmrxmhz.html

Go:   "第一行\n第二行"
来源：http://hz.sweek.top/gtgxdkynpr.html

Ruby: "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtqxucvcmy.html

C#:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtqxmlgqak.html

[A14] 注释写法
来源：http://hz.feifeiyinyue.top/gtysxovyyw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.gaohongyu789.top/gtrbgjcdpa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hammf.cn/gtoolmidhz.html

JS:   // 单行；/* 多行 */
来源：http://hz.hywenlv.cn/gthberftgo.html

TS:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gtlonypuxc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.cashguo.top/gtmkoesmnd.html

Go:   // 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtwjmegqdd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.chenjidiqi.icu/gtklwjntbp.html

C#:   // 单行；/* 多行 */
来源：http://hz.xziqi.cn/gtlhgaffmk.html

[A15] 空值判断与默认值
来源：http://hz.pycfn.com/gtkwmauwda.html

Py:   value = data or "默认值"
来源：http://hz.vqdsnc.cn/gtusmgxaug.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zdqjudy.top/gtghwojlzp.html

JS:   const value = data ?? "默认值";
来源：http://hz.hysaishi.cn/gtuwrgagte.html

TS:   const value = data ?? "默认值";
来源：http://hz.xziqi.cn/gtgtumyiud.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.guannengcc.top/gtlppdupsh.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shanyushiyangkeji.top/gtvfiwhbfk.html

Ruby: value = data || "默认值"
来源：http://hz.gotoacloud.top/gtusshkhuk.html

C#:   var value = data ?? "默认值";
来源：http://hz.wangdashe.top/gtplimprtb.html

[A16] 真假值判断规则
来源：http://hz.kuanghao11.cn/gtehzcdjqg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.kuanghao11.cn/gtrpjqovtv.html


<!-- 参考信息 -->