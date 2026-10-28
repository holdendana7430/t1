代发 wailian999

[U93] JS：模板字符串
来源：http://hz.cheryme.top/gtretocpdn.html

`共 ${n} 条`
来源：http://hz.zhaomingkeji.xyz/gtjxhsdplp.html

[U94] JS：箭头函数
来源：http://hz.zhongyouzk.top/gtffzvmxcw.html

const double = x => x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtzlpdzmnd.html

[U95] JS：Promise 包装
来源：http://hz.cdnleiting.top/gtowxjclgm.html

new Promise((resolve, reject) => {})
来源：http://hz.316326.xyz/gteyfjegor.html

[U96] JS：async/await 与异常
来源：http://hz.cdnleiting.top/gtrglykrjy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gthphlrmjj.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtxlwnvctj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtkeeymbkt.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtixfxcyrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258888.top/gtpksurrdw.html

[U99] JS：事件监听
来源：http://hz.0kj1m.cn/gtszypnkdu.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtprtvabpm.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtbeyoimyy.html

document.querySelector(".item")
来源：http://hz.yj20258888.top/gtgptoekuw.html

[U101] JS：classList 操作
来源：http://hz.yonumen.top/gthpiipwkc.html

el.classList.toggle("active")
来源：http://hz.cashguo.top/gthyawspko.html

[U102] JS：本地存储
来源：http://hz.aizwys.cn/gthtebhqxd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtjqmzshss.html

[U103] JS：定时器
来源：http://hz.hongshengwenyu.top/gtpmjzfcyt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guowangkeji.top/gtrnxmffri.html

[U104] JS：防抖
来源：http://hz.jinqigfzy.top/gtzsaqtdph.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtlskeljuq.html

[U105] JS：节流
来源：http://hz.gotoacloud.top/gtiyhrwouz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.quarkkingdee.top/gtwpbyffvn.html

[U106] JS：日期格式化
来源：http://hz.cucudq.cn/gtbqwndsol.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258888.top/gtqubffvte.html

[U107] JS：数字千分位
来源：http://hz.mhx1999.top/gtypudosvf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sxryk.cn/gtistjelpn.html

[U108] JS：随机整数
来源：http://hz.gotoacloud.top/gteginaten.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtnzoblazm.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtucnfudcn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtmoudsywh.html

[U110] JS：数组分块
来源：http://hz.kuanghao11.cn/gtjobwoqba.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cheryme.top/gtymukkzei.html

[U111] JS：对象转 Map
来源：http://hz.fzhhl.top/gtovzmxcyg.html

new Map(Object.entries(obj))
来源：http://hz.jinqigfzy.top/gttitnoqhy.html

[U112] JS：字符串补位
来源：http://hz.yanxiufei.cn/gtqiuyuddf.html

"7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtracevffb.html

[U113] JS：正则替换全部
来源：http://hz.hongshengwenyu.top/gtpmqpjmcx.html

s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtkryobbvq.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtjjqgdhtt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtnctkrxpt.html

[U115] JS：生成 UUID
来源：http://hz.fengsongda.top/gtdsxtuqky.html

crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtweybxbuf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.kuanghao11.cn/gtsragzozj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sufxvd.cn/gtqxvefnyk.html

[U117] JS：单元测试
来源：http://hz.cqqwz.cn/gtsdichurz.html

npm i -D vitest;  npx vitest
来源：http://hz.yueranfly.top/gtcxffyhal.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangtech.top/gtmrxqyoju.html

npm i -D vite;  npx vite
来源：http://hz.c1oappe.top/gtgfvwoiws.html

[U119] JS：生产构建
来源：http://hz.vqdsnc.cn/gtbcxgnqja.html

npx vite build
来源：http://hz.ehwqpu.com/gtnraobxux.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hfpthk.cn/gtuiweunik.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtyctnjzdk.html

================================================================================
来源：http://hz.iojbl.cn/gtdnmrptrn.html

统计汇总
来源：http://hz.yuxming.cn/gtnyqaktkx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmqsqdgti.html

按语言统计（条）：
来源：http://hz.aizwys.cn/gtzoxewbso.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gtiwqvjvor.html

PHP ............ 252
来源：http://hz.meibo888.top/gtizyqgrgw.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gtyynrldbu.html

TypeScript ..... 212
来源：http://hz.redwolf501.top/gtaccwfmpn.html

Java ........... 212
来源：http://hz.tanke756.top/gthpxoccgn.html

Go ............. 212
来源：http://hz.zycfv.cn/gttgcwxtlx.html

Ruby ........... 212
来源：http://hz.nanxinkj.top/gtddeylxmg.html

C# ............. 212
来源：http://hz.hywenlv.cn/gtecetctxe.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtikplqmpx.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtffikshyg.html

SQL ............ 90
来源：http://hz.aizwys.cn/gtazcbdcuw.html

Bash ........... 80
来源：http://hz.yj20258.top/gtnksacrrw.html

Kotlin ......... 15
来源：http://hz.yvedp.cn/gtxgtlucpb.html

Swift .......... 15
来源：http://hz.jqgfzy.top/gtelcwzfzs.html

Lua ............ 10
来源：http://hz.sxryk.cn/gtwbqvrqer.html

Perl ........... 10
来源：http://hz.gzhubu.top/gtctusyxkq.html

Scala .......... 10
来源：http://hz.xingfuxueyuan.xyz/gtaptsinra.html

------------------------------------
来源：http://hz.gzhubu.top/gtchxdbwzh.html

合计 ........... 2106 条
来源：http://hz.dashuyun.cn/gtigcxoeth.html

按章节统计：
来源：http://hz.yj20258.top/gtwbqdcppk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtniqnwgue.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtngjtdopv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gtcepdqdiu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtbyhxyaha.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shzxlz.cn/gtwjdrwmuh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtllowuzlw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtsfbzsmqm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydjk.org.cn/gthojkxvgg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtomnfsoti.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj202588.top/gtutcfhynd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtqjpsgbai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtasmwicqz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtcxdatwlw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.meibo888.top/gtyzeiyfyh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.guannengcc.top/gtgwsiacwk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtqsaofpyl.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gttewmwesu.html

R Bash 专题                             80
来源：http://hz.chenzaomai.com/gtzignenay.html

S C / C++ 专题                          60
来源：http://hz.smart0.xyz/gtzordjsdl.html

T 其他语言补充                          60
来源：http://hz.shuidangran.top/gtlqhtwhtd.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gteigrjjgh.html

------------------------------------
来源：http://hz.kuanghao11.cn/gtjmlxynok.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtixfeltkf.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtpwlzqwdd.html

使用提醒
来源：http://hz.wangdashe.top/gtifoumjyg.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtigjafxlj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sysykeji.top/gtjojolrsv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj202588.top/gtluoinvqx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenjidiqi.icu/gtbazxtvkr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jlsjyb.cn/gticyooqxb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.svipenyu.cn/gtdwrnzeuc.html

—— 文件结束 ——
来源：http://hz.yj202588.top/gtmcxsciot.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmqzqjfox.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hongshengwenyu.top/gtkkjvmhpi.html

Common Programming Examples Cheat Book
来源：http://hz.pycfn.com/gtmpuxnmyf.html

================================================================================
来源：http://hz.sufxvd.cn/gtupnklxrm.html

【收录内容】
来源：http://hz.quarkkingdee.top/gtdmcmuwcw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cheryme.top/gtlauixmij.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhiwuduotai.top/gtgembuzwj.html

SQL · Bash · C · C++
来源：http://hz.ywan-chungtsiang.top/gtuhotqlle.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuanzx.com/gtucbnifyf.html

【使用说明】
来源：http://hz.nanxuanxn.top/gtdqggpggv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nwbrower.top/gtjcpqsroz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinqigufen.top/gttolxcfpj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nwbrower.top/gtclrwovgl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pengpengdd.cyou/gtcrwlibot.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.snrcjt.cn/gtdzysszdp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gzhubu.top/gtegomvhhu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yongpay.top/gtbarjspko.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cashguo.top/gtifqolnar.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shanyushiyangtech.top/gtvuucgdih.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gotoacloud.top/gtbeoxirku.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dashuyun.cn/gttvkcsbrt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tian-w.cn/gtvflumtvb.html

【文件统计】
来源：http://hz.dianchejie.cn/gtrhpafkrr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hongshengwenyu.top/gtxuwzfprs.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtumbwoidf.html

目  录
来源：http://hz.fengsongda.top/gtejxmsdyz.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtyqnwanrr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtpekmuynx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtkmajdflq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtfgmolkrl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gtyqtiwyhe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yongpay.top/gtuidrnmfs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.daxiang520.top/gtqeegbrtr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhoulong.xyz/gtsxffoily.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tianlin.xyz/gtrlgqsbzi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dashuyun.cn/gtocuplcwj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.quarkkingdee.top/gtwxaxhexu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gthqttjopu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtsulbwlwt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtryabzdkz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.guannengcc.top/gtrzfstqjg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinqigfzy.top/gtroiodtpd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtxwsqocqs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dashuyun.cn/gtuaknafej.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.vqdsnc.cn/gtbdtvryfm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xuanzx.com/gtaquhuhap.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtirmircal.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtnflbggta.html

================================================================================
来源：http://hz.ivvv.top/gtxuevjgys.html

A. 基础语法与类型
来源：http://hz.hfpthk.cn/gtoqcakzlw.html

================================================================================
来源：http://hz.daxiang520.top/gtqstybzun.html

[A01] Hello World
来源：http://hz.shangyingyoupin.top/gtlrlsvmlf.html

Py:   print("Hello, World!")
来源：http://hz.sysykeji.top/gtnlunbrbh.html

PHP:  echo "Hello, World!";
来源：http://hz.jianghu66.top/gtbewmilrr.html

JS:   console.log("Hello, World!");
来源：http://hz.sysykeji.top/gtcaloyryv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.pycfn.com/gtijsagaiq.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj202588.top/gtrrtauyqc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ivvv.top/gtaeezcckj.html

Ruby: puts "Hello, World!"
来源：http://hz.jinyuanbaomall.cn/gtlhnwscks.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuanzhike.top/gtasvcratm.html

[A02] 变量声明与赋值
来源：http://hz.jinqigfzy.top/gttpzbpufz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yanxiufei.cn/gtjdmydndg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sufxvd.cn/gtgtjmftva.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yonumen.top/gtenpfxyvu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhijiandao.cn/gtakorjfes.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangtech.top/gtnpqpbxwk.html

Go:   name := "Alex"; age := 20
来源：http://hz.yongpay.top/gtjxxndgrl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.dianchejie.cn/gtkhkehxht.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtydxuizjq.html

[A03] 常量定义
来源：http://hz.zhengqikj.top/gtnqpnnfwp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ehwqpu.com/gteblzgdfz.html

PHP:  const PI = 3.14159;
来源：http://hz.yuanzhike.top/gthhwvdbhb.html

JS:   const PI = 3.14159;
来源：http://hz.nwbrower.top/gtbvqxiexg.html

TS:   const PI: number = 3.14159;
来源：http://hz.quarkkingdee.top/gtyfxsdzto.html

Java: static final double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtrthvtqxx.html

Go:   const PI = 3.14159
来源：http://hz.pengpengdd.cyou/gtiwkpwkwz.html

Ruby: PI = 3.14159
来源：http://hz.shuidangran.top/gtvuvbxyhf.html

C#:   const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gttqxlpwgn.html

[A04] 判断变量类型
来源：http://hz.hongshengwenyu.top/gtwzdehmft.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxuanxn.top/gtpepnpptp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xuetiantiany.cn/gtoelhsffu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hysaishi.cn/gtvuqhnubp.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangdashe.top/gtjkupzrlq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.fzhhl.top/gtwqtogfza.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hywenlv.cn/gtjyuujyix.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gtbeibgbqo.html

C#:   x.GetType().Name; x is int
来源：http://hz.redwolf501.top/gtplegebbc.html

[A05] 整数除法与取模
来源：http://hz.havefunace.top/gthkperivz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jqgufenzy.top/gtuinaoryk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtashatxyi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj202588.top/gtpgxlobby.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtbutjkbnx.html

Java: 7 / 2; 7 % 2
来源：http://hz.sxryk.cn/gtrthmdvjy.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtzkphijod.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtviyynvan.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtikwgihwv.html

[A06] 字符串转数字
来源：http://hz.jiagoushi.top/gtmrkjxqsm.html

Py:   int("42"); float("3.14")
来源：http://hz.pycfn.com/gtwnpoqgrn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.nanxuanxn.top/gtqdwcjnpz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.9152youxi.cn/gthfokdvxv.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtjjhsybtt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinqigfzy.top/gtkqvxjjqd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtcsqkijwk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgfzy.top/gteugapxgo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangshuangyany.cn/gtfgxdlksc.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtuwtowwua.html

Py:   str(42)
来源：http://hz.ivvv.top/gtfhrwrmhe.html

PHP:  (string) 42; strval(42)
来源：http://hz.andypj.xyz/gtfwkhnbad.html

JS:   String(42); (42).toString()
来源：http://hz.wangdashe.top/gtiatjnuyp.html

TS:   String(42)
来源：http://hz.zhoulong.xyz/gtdjqhubqs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.redwolf501.top/gtjedcshzg.html

Go:   strconv.Itoa(42)
来源：http://hz.hywenlv.cn/gtzrmpjzjx.html

Ruby: 42.to_s
来源：http://hz.jinghuilouyu.cn/gtuqpqfgua.html

C#:   42.ToString()
来源：http://hz.52xcode.cn/gtndapmvrc.html

[A08] 取整与四舍五入
来源：http://hz.snrcjt.cn/gtwrxxfvhm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.dashuyun.cn/gtzivxizvi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.feifeiyinyue.top/gtjpqfmbix.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hammf.cn/gtyccdsqfx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ywan-chungtsiang.top/gtzcyvzqlj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.316326.xyz/gtisehcsnt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cucudq.cn/gtxivghdkd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.9152youxi.cn/gtvrxizcbm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yuanzhike.top/gtpbkihogr.html

[A09] 绝对值与最大最小值
来源：http://hz.zhaomingkeji.xyz/gtfktrcodr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtkgjiyxqu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shzxlz.cn/gtvbbvrmfe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.wangshuangyany.cn/gtvlaclzkk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gtsnhsfuww.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhengqikj.top/gtnhyrlpoa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinyuanbaomall.cn/gtjfsumigp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hnxiangtu.top/gtjalsrrrf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hfpthk.cn/gtmnncckoz.html

[A10] 生成随机数
来源：http://hz.guannengcc.top/gtagdudwki.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jinqigfzy.top/gtmnwwruuq.html

PHP:  random_int(1, 100);
来源：http://hz.cashguo.top/gttsvaqaad.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ybcxt.top/gtrltbzvyd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuxming.cn/gtyhxrwayi.html

Java: new Random().nextInt(100) + 1
来源：http://hz.0kj1m.cn/gtxrikzopu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinqigfzy.top/gtdarfqnxd.html

Ruby: rand(1..100)
来源：http://hz.yongpay.top/gtebehexqo.html

C#:   new Random().Next(1, 101)
来源：http://hz.yongpay.top/gtnjktonym.html

[A11] 条件表达式（三元）
来源：http://hz.zdqjudy.top/gtiyfnnizf.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yangfankeji.com/gtvxztdcpz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtaipenehw.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtnafobsgp.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtbzfogcdy.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtzbrykhev.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xingfuxueyuan.xyz/gtirnblime.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtwqfvrsqh.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtkasbhmfi.html

[A12] 字符串插值 / 格式化
来源：http://hz.shangyingyoupin.top/gtyqgrvxmh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jqgfzy.top/gtcibqjsvr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sysykeji.top/gtqqsrqydi.html

JS:   `Hello, ${name}!`
来源：http://hz.tianlin.xyz/gthybbzdca.html

TS:   `Hello, ${name}!`
来源：http://hz.ivvv.top/gtzhslnkpk.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ydjk.org.cn/gtdddzqcgz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.cheryme.top/gtgsvbojpu.html

Ruby: "Hello, #{name}!"
来源：http://hz.jlsjyb.cn/gtezsuhywn.html

C#:   $"Hello, {name}!"
来源：http://hz.yj20258.top/gthpawqphb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.wangshuangyany.cn/gtcjfzsihj.html

Py:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtcyxndqpn.html

PHP:  "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtwkvhruiq.html

JS:   "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtcdfaibbc.html

TS:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtdtoertor.html

Java: "第一行\n第二行"
来源：http://hz.wangdashe.top/gtcljyvfoa.html

Go:   "第一行\n第二行"
来源：http://hz.pycfn.com/gtsjznlpob.html

Ruby: "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtonfjbgmp.html

C#:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtunzcvohm.html

[A14] 注释写法
来源：http://hz.xylfe.cn/gtguegpanm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yuanzhike.top/gthwuqppca.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtvloesotw.html

JS:   // 单行；/* 多行 */
来源：http://hz.xinyue.icu/gtxgoimrnh.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhijiandao.cn/gtpvvzihyp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.gotoacloud.top/gtxkzyawbb.html

Go:   // 单行；/* 多行 */
来源：http://hz.yj20258888.top/gtgkmyqfel.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jlsjyb.cn/gtsikkjedt.html

C#:   // 单行；/* 多行 */
来源：http://hz.mhx1999.top/gtuvzlsaxj.html

[A15] 空值判断与默认值
来源：http://hz.shangyingyoupin.top/gtdpiarrcb.html

Py:   value = data or "默认值"
来源：http://hz.jinqigfzy.top/gtlvplihfs.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.gaohongyu789.top/gtrenvujdb.html

JS:   const value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtxcjyiaxw.html

TS:   const value = data ?? "默认值";
来源：http://hz.andypj.xyz/gtkwghemgp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.iojbl.cn/gtnkqyacjx.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.guannengcc.top/gtupysofrx.html

Ruby: value = data || "默认值"
来源：http://hz.hywenlv.cn/gtutdzuivw.html

C#:   var value = data ?? "默认值";
来源：http://hz.aizwys.cn/gtbytgewnf.html

[A16] 真假值判断规则
来源：http://hz.zdqjudy.top/gtjzsdurdf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dianchejie.cn/gtthcuktoo.html


<!-- 参考信息 -->