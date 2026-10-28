代发 wailian999

[U95] JS：Promise 包装
来源：http://hz.hammf.cn/gtbeiyzyts.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtbaxiagtw.html

[U96] JS：async/await 与异常
来源：http://hz.yanxiufei.cn/gtkiwfuplm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtvhfxksvl.html

[U97] JS：并发请求
来源：http://hz.redwolf501.top/gtfmjkvtex.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtvjnbaguu.html

[U98] JS：fetch 带 JSON
来源：http://hz.shangyingyoupin.top/gtusgothir.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenjidiqi.icu/gtxnxcnqqh.html

[U99] JS：事件监听
来源：http://hz.pengpengdd.cyou/gtkjueupjn.html

el.addEventListener("click", e => {})
来源：http://hz.0kj1m.cn/gtxkhvtlyq.html

[U100] JS：DOM 查询
来源：http://hz.ydzc1.top/gtgzxfmyco.html

document.querySelector(".item")
来源：http://hz.chenzaomai.com/gtffblagyf.html

[U101] JS：classList 操作
来源：http://hz.feifeiyinyue.top/gtdtxqwylq.html

el.classList.toggle("active")
来源：http://hz.chenjidiqi.icu/gthivkefpz.html

[U102] JS：本地存储
来源：http://hz.sxryk.cn/gtsjqsjotl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.daria6918.cn/gtbhbiczbq.html

[U103] JS：定时器
来源：http://hz.zycfv.cn/gtkvxcully.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ehwqpu.com/gtomjpdpbx.html

[U104] JS：防抖
来源：http://hz.zdqjudy.top/gtzkzpdhlr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtkbwqzjju.html

[U105] JS：节流
来源：http://hz.cdnleiting.top/gtgeojwhyf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.iojbl.cn/gtcyyqdgdf.html

[U106] JS：日期格式化
来源：http://hz.sufxvd.cn/gtzbbqpgim.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gaohongyu789.top/gtdnjqdfmw.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gtqzsffewr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgufenzy.top/gtmuecflry.html

[U108] JS：随机整数
来源：http://hz.fengsongda.top/gtuijrrbbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtdyqevodg.html

[U109] JS：数组分组
来源：http://hz.chenzaomai.com/gttyrofatb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtsdccogxy.html

[U110] JS：数组分块
来源：http://hz.smart0.xyz/gtbkbhtbcg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.feifeiyinyue.top/gtjzefnyqx.html

[U111] JS：对象转 Map
来源：http://hz.jinqigufen.top/gtoucnxeou.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtilkdrmob.html

[U112] JS：字符串补位
来源：http://hz.tanke756.top/gtbddmoihp.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtcdsecpdb.html

[U113] JS：正则替换全部
来源：http://hz.snrcjt.cn/gtunujtdxe.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtwyvtqfvt.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtgkloxiup.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtdstoazfs.html

[U115] JS：生成 UUID
来源：http://hz.ppjwa.cn/gtfkzuznec.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtpmbtstwn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yonumen.top/gtrlgyhyoh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhengqikj.top/gtxheozmzr.html

[U117] JS：单元测试
来源：http://hz.hnxiangtu.top/gtjtmizcnb.html

npm i -D vitest;  npx vitest
来源：http://hz.daxiang520.top/gtlwxytsxx.html

[U118] JS：开发服务器
来源：http://hz.yanxiufei.cn/gtuviyljdu.html

npm i -D vite;  npx vite
来源：http://hz.ydzc1.top/gtxfnvmpxx.html

[U119] JS：生产构建
来源：http://hz.yj202588.top/gtvbvvwhxw.html

npx vite build
来源：http://hz.yj20258888.top/gtkfjnkydp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtctjnbbcm.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gttpxjbxcf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsdfmztaf.html

统计汇总
来源：http://hz.gaohongyu789.top/gtxlfjdczl.html

================================================================================
来源：http://hz.tian-w.cn/gtronncafo.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtqedjtskw.html

Python ......... 252
来源：http://hz.sufxvd.cn/gthfcahalo.html

PHP ............ 252
来源：http://hz.jinyuanbaomall.cn/gtjdkafzgz.html

JavaScript ..... 252
来源：http://hz.316326.xyz/gtqltwvxak.html

TypeScript ..... 212
来源：http://hz.9152youxi.cn/gtdguvbviz.html

Java ........... 212
来源：http://hz.zdqjudy.top/gtofaytazp.html

Go ............. 212
来源：http://hz.yvedp.cn/gtkhcuvvnq.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gtzjcjsrtz.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtiupztgkc.html

C .............. 30
来源：http://hz.yj20258888.top/gtvktakplt.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtdqeuuejm.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtcvokendd.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtcsaryvmq.html

Kotlin ......... 15
来源：http://hz.xuetiantiany.cn/gtrdbrvwps.html

Swift .......... 15
来源：http://hz.sufxvd.cn/gtbqdnqfot.html

Lua ............ 10
来源：http://hz.aizwys.cn/gtnvtbqcju.html

Perl ........... 10
来源：http://hz.chenlongwang.top/gtkdvepcst.html

Scala .......... 10
来源：http://hz.svipenyu.cn/gtaqwdsowg.html

------------------------------------
来源：http://hz.cqqwz.cn/gtwumkqhms.html

合计 ........... 2106 条
来源：http://hz.shangyingyoupin.top/gtyeavofqp.html

按章节统计：
来源：http://hz.shuidangran.top/gthnptumsk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtiuezdtsi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shuidangran.top/gtstaohabm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtgiddfxvh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtzuwbujac.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yangfankeji.com/gtuhhowhrs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtgwpjmnsk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtnubdgfgm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dashuyun.cn/gttrhwgsom.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtoexdkmxw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydjk.org.cn/gtfprujogn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtmwplwmyw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtikizqnzs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtckossocs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.feifeiyinyue.top/gtbjviuada.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daria6918.cn/gtwtxgnkzc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtjuorbhoz.html

Q SQL 专题                              90
来源：http://hz.cqqwz.cn/gtbrurskvf.html

R Bash 专题                             80
来源：http://hz.zhixingplan.top/gtrhbkyien.html

S C / C++ 专题                          60
来源：http://hz.mhx1999.top/gtczbijeka.html

T 其他语言补充                          60
来源：http://hz.sufxvd.cn/gtgcqubudr.html

U 高频实用片段                         120
来源：http://hz.xylfe.cn/gtpxzrxoxc.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtecdidxdl.html

合计                                  2106 条
来源：http://hz.yj20258.top/gtselkmhui.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gtxqlbqcrc.html

使用提醒
来源：http://hz.sxryk.cn/gtuxhccqfm.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtvymkjllu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jiagoushi.top/gtuupeyahd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sysykeji.top/gtaqifsgor.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuetiantiany.cn/gtuqipoyje.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gthxxufwnv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yuanzhike.top/gtasewcyzv.html

—— 文件结束 ——
来源：http://hz.meibo888.top/gteheshqph.html

================================================================================
来源：http://hz.havefunace.top/gtxebzkezg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.fzhhl.top/gtgroupgfb.html

Common Programming Examples Cheat Book
来源：http://hz.hfpthk.cn/gtqtpfkdwv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtphzujooc.html

【收录内容】
来源：http://hz.sweek.top/gtklmzvuqb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pycfn.com/gttdbgmokv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtyidlnjvd.html

SQL · Bash · C · C++
来源：http://hz.fzhhl.top/gtvcpsttvt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jqgufenzy.top/gtefjfnlqu.html

【使用说明】
来源：http://hz.ivvv.top/gtalqounel.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtyuubjxvf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zycfv.cn/gtwmaukebr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.redwolf501.top/gtlnbcumff.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtvzxuryci.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxuanxn.top/gtdojoveqw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhixingplan.top/gtwfnrspda.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gttxwumtjo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hammf.cn/gtizbqtptj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtcnhpgelg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gtuyeqytcw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtisqkleln.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhaomingkeji.xyz/gtjigeqnaq.html

【文件统计】
来源：http://hz.yueranfly.top/gtmnmiakvk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dashuyun.cn/gtsubzjqpt.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtsqlofswl.html

目  录
来源：http://hz.sufxvd.cn/gtqfwiofnn.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtgptntyvc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gttvoruyrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtiuthjsei.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtgdqsiwmp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.kuanghao11.cn/gttotsqutp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuanzhike.top/gtnkbqehox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pengpengdd.cyou/gterqhtxih.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtqgafmhje.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.9152youxi.cn/gttuvlrzds.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtflrufzgg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangkeji.top/gtjzebwngm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtahnblshk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtswmppoeb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtcphysput.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtriilbhvi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sweek.top/gtuwknnykc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtegtnfixm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jqgufenzy.top/gtxgdzugyp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhijiandao.cn/gtcstpuiwj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hywenlv.cn/gtvrgkxmno.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtmlydwshj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtxpocjzxc.html

================================================================================
来源：http://hz.hammf.cn/gtolmvecbv.html

A. 基础语法与类型
来源：http://hz.ywan-chungtsiang.top/gtmjuszlah.html

================================================================================
来源：http://hz.dashuyun.cn/gtjbhyofuw.html

[A01] Hello World
来源：http://hz.hammf.cn/gtxfgeyime.html

Py:   print("Hello, World!")
来源：http://hz.c1oappe.top/gtkfmdndyu.html

PHP:  echo "Hello, World!";
来源：http://hz.jiagoushi.top/gtvfjkbgla.html

JS:   console.log("Hello, World!");
来源：http://hz.shzxlz.cn/gtsikhwvti.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xziqi.cn/gtbfwubmsi.html

Java: System.out.println("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtwbmqovla.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cqqwz.cn/gtqbotavgv.html

Ruby: puts "Hello, World!"
来源：http://hz.zhongyouzk.top/gtokjfxggg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zycfv.cn/gtezlohedr.html

[A02] 变量声明与赋值
来源：http://hz.meibo888.top/gthdarcsdr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.snrcjt.cn/gtdjsnuorg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gogol.net.cn/gtpdyawqnu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yongpay.top/gthwvoipin.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.birdmap.top/gtmqlccyqt.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shzxlz.cn/gtefaamjbz.html

Go:   name := "Alex"; age := 20
来源：http://hz.yonumen.top/gtormpunfy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cdnleiting.top/gtotrmvwbi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.andypj.xyz/gtzdbztfyl.html

[A03] 常量定义
来源：http://hz.wangshuangyany.cn/gtuaxjefya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xinyue.icu/gtimneellg.html

PHP:  const PI = 3.14159;
来源：http://hz.iojbl.cn/gtldfgvehe.html

JS:   const PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtgunrntgt.html

TS:   const PI: number = 3.14159;
来源：http://hz.vqdsnc.cn/gtuxrysrbi.html

Java: static final double PI = 3.14159;
来源：http://hz.daxiang520.top/gteflvlpbh.html

Go:   const PI = 3.14159
来源：http://hz.guowangkeji.top/gtiqvdorfb.html

Ruby: PI = 3.14159
来源：http://hz.hongshengwenyu.top/gtwnirvcsu.html

C#:   const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtdqkbfxwh.html

[A04] 判断变量类型
来源：http://hz.hnxiangtu.top/gtvjgzwmge.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.bjfxy.top/gtbuvpcnmb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gtowfzvlfs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sufxvd.cn/gtlvlgcmef.html

TS:   typeof x; x instanceof Date
来源：http://hz.sweek.top/gtiwiklwrv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jianghu66.top/gtvirfxzlo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.wangdashe.top/gtqvnzondr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.snrcjt.cn/gtdegeevcz.html

C#:   x.GetType().Name; x is int
来源：http://hz.hfpthk.cn/gthqpmiyrg.html

[A05] 整数除法与取模
来源：http://hz.redwolf501.top/gtlgvxdwym.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxinkj.top/gtbsveywer.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.dashuyun.cn/gtfkdveusd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sysykeji.top/gttxcleygo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jyoumei.cn/gttjzawbmk.html

Java: 7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtpdougrbm.html

Go:   7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtrgfgrlbr.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtlcyedxnn.html

C#:   7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtdknhjiba.html

[A06] 字符串转数字
来源：http://hz.svipenyu.cn/gtnttzkopu.html

Py:   int("42"); float("3.14")
来源：http://hz.cdnleiting.top/gtfbvecbjw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hongshengwenyu.top/gtuutkeccd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yonumen.top/gtijoypjer.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xylfe.cn/gtddofkjbi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.9152youxi.cn/gtodeyxvou.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ywan-chungtsiang.top/gtfutuzopb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.guannengcc.top/gtljxulrnq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.meibo888.top/gtdbeuntpi.html

[A07] 数字转字符串
来源：http://hz.9152youxi.cn/gtyjjngvmm.html

Py:   str(42)
来源：http://hz.ehwqpu.com/gtwuwbxbnd.html

PHP:  (string) 42; strval(42)
来源：http://hz.ppjwa.cn/gtxghajsta.html

JS:   String(42); (42).toString()
来源：http://hz.dashuyun.cn/gtgongwjen.html

TS:   String(42)
来源：http://hz.sufxvd.cn/gtpfalgqay.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ydzc1.top/gtoxfxbhgs.html

Go:   strconv.Itoa(42)
来源：http://hz.vqdsnc.cn/gtprpgqjzf.html

Ruby: 42.to_s
来源：http://hz.kuanghao11.cn/gtsgbigggr.html

C#:   42.ToString()
来源：http://hz.dianchejie.cn/gtyhoqekuw.html

[A08] 取整与四舍五入
来源：http://hz.daxiang520.top/gtexkcaqee.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.daria6918.cn/gtltjjbrzm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yuanzhike.top/gtitmbugii.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shangyingyoupin.top/gtvgzsfdle.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.tanke756.top/gtbqrghdcl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.c1oappe.top/gtxsswtsgz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.guowangkeji.top/gtjjyhwpyl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ydjk.org.cn/gtyulbsnlo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.vqdsnc.cn/gtcksiewep.html

[A09] 绝对值与最大最小值
来源：http://hz.gotoacloud.top/gtttinsxyc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hysaishi.cn/gtpemwdiap.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj202588.top/gtrfqhkikk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.sxryk.cn/gtvjopsfrx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jiagoushi.top/gtcfmbuyhw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtyrngybbo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinqigufen.top/gtcoqhlfnj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.meibo888.top/gtmrawdvyc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.redwolf501.top/gtrpbopcog.html

[A10] 生成随机数
来源：http://hz.svipenyu.cn/gtsmkurhrp.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sxryk.cn/gtwopcwijy.html

PHP:  random_int(1, 100);
来源：http://hz.52xcode.cn/gtkcjnrkvr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.feifeiyinyue.top/gtoqvsodwo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ywan-chungtsiang.top/gtcwonbxki.html

Java: new Random().nextInt(100) + 1
来源：http://hz.52xcode.cn/gtfaervbxg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ybcxt.top/gtvytztmvx.html

Ruby: rand(1..100)
来源：http://hz.redwolf501.top/gtazzzwuar.html

C#:   new Random().Next(1, 101)
来源：http://hz.ybcxt.top/gtdgcknxlb.html

[A11] 条件表达式（三元）
来源：http://hz.quarkkingdee.top/gtzcsuogeh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtczezrmht.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtrfuolecz.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ehwqpu.com/gtzlswtwdk.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtcqbjybys.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtfdusxtts.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.iojbl.cn/gttantudgj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.daria6918.cn/gtmoroqebj.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtzjwbzgcn.html

[A12] 字符串插值 / 格式化
来源：http://hz.hnqzz.top/gtwzkorhvr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hnqzz.top/gtxhvceynx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zdqjudy.top/gtdtpnydfd.html

JS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtjrxkftvs.html

TS:   `Hello, ${name}!`
来源：http://hz.hnqzz.top/gtftfeuixy.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.chenjidiqi.icu/gtxarfbvjo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.0kj1m.cn/gtbacfsudr.html

Ruby: "Hello, #{name}!"
来源：http://hz.nanxuanxn.top/gtrmmayswz.html

C#:   $"Hello, {name}!"
来源：http://hz.dianchejie.cn/gtlakwqpmk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ehwqpu.com/gtvotmkvih.html

Py:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtiktlqovy.html

PHP:  "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gttrljdbwz.html

JS:   "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtapvwfowp.html

TS:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtkbogeyxr.html

Java: "第一行\n第二行"
来源：http://hz.iojbl.cn/gtzpoxqhrs.html

Go:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtcevdbopr.html

Ruby: "第一行\n第二行"
来源：http://hz.yongpay.top/gtcopwvrtl.html

C#:   "第一行\n第二行"
来源：http://hz.fzhhl.top/gtskhmatur.html

[A14] 注释写法
来源：http://hz.shangyingyoupin.top/gtpjbubdup.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.9152youxi.cn/gtniqpeayl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.meibo888.top/gtakbnludl.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhijiandao.cn/gtsyikxvkl.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtrleiseih.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.ydjk.org.cn/gtegxgpikr.html

Go:   // 单行；/* 多行 */
来源：http://hz.andypj.xyz/gtkvazrpjs.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.birdmap.top/gtkwhrnypc.html

C#:   // 单行；/* 多行 */
来源：http://hz.zdqjudy.top/gtosxdkmzw.html

[A15] 空值判断与默认值
来源：http://hz.hfpthk.cn/gtphlwjjrr.html

Py:   value = data or "默认值"
来源：http://hz.xylfe.cn/gtqcrsncyk.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.iojbl.cn/gtxzarjifj.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhiwuduotai.top/gtiabtjpxy.html

TS:   const value = data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtgtpikxeq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jlsjyb.cn/gtkpcpftpe.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jinqigufen.top/gtywhdnbgv.html

Ruby: value = data || "默认值"
来源：http://hz.mhx1999.top/gtzohmklrw.html

C#:   var value = data ?? "默认值";
来源：http://hz.316326.xyz/gtrikguncb.html

[A16] 真假值判断规则
来源：http://hz.nanxuanxn.top/gtaobvdeqj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.gaohongyu789.top/gtfuempqlk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jqgfzy.top/gtvuxtttqv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yj20258.top/gtrvkauaql.html

TS:   if (!x) {}
来源：http://hz.shangyingyoupin.top/gtlefzhkrd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.xingfuxueyuan.xyz/gtioseuziq.html


<!-- 参考信息 -->