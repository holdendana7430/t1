代发 wailian999

[U87] JS：解构默认值
来源：http://hz.hongshengwenyu.top/gtbezwmexq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnxiangtu.top/gthtyrvnfo.html

[U88] JS：对象展开合并
来源：http://hz.haohaochexian.top/gtpcrdspqa.html

{ ...a, ...b }
来源：http://hz.bjfxy.top/gtoqohvyvt.html

[U89] JS：数组去重
来源：http://hz.hongshengwenyu.top/gtvwpwvlvl.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtiwymscwq.html

[U90] JS：数字数组排序
来源：http://hz.yuxming.cn/gtjgyskfuq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtarocrgll.html

[U91] JS：对象键值遍历
来源：http://hz.jianghu66.top/gtcsdjwgrg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sufxvd.cn/gtifiegwbo.html

[U92] JS：深拷贝
来源：http://hz.havefunace.top/gtwhbtezdv.html

structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtjufniibc.html

[U93] JS：模板字符串
来源：http://hz.kuanghao11.cn/gtwrxwgdmy.html

`共 ${n} 条`
来源：http://hz.jianghu66.top/gtxqltdbwb.html

[U94] JS：箭头函数
来源：http://hz.jinqigufen.top/gtiwbtskef.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtgtvmnojx.html

[U95] JS：Promise 包装
来源：http://hz.zdqjudy.top/gtfpjwzett.html

new Promise((resolve, reject) => {})
来源：http://hz.zhengqikj.top/gtmgsogeuy.html

[U96] JS：async/await 与异常
来源：http://hz.jlsjyb.cn/gtcvbayepr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtecgtirlw.html

[U97] JS：并发请求
来源：http://hz.tianlin.xyz/gtrfulshqz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtdwqxfpyh.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydzc1.top/gtyrlxuiyw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.dashuyun.cn/gtopiyfvno.html

[U99] JS：事件监听
来源：http://hz.wangshuangyany.cn/gttdqhghhu.html

el.addEventListener("click", e => {})
来源：http://hz.zycfv.cn/gtvjllkene.html

[U100] JS：DOM 查询
来源：http://hz.sufxvd.cn/gtwxioabwd.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtenllevpj.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gtwsbywjgz.html

el.classList.toggle("active")
来源：http://hz.hnqzz.top/gtktbhydeu.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtnirrmqsd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.andypj.xyz/gthsdwtbct.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtotiejwgt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jianghu66.top/gtyagqxbem.html

[U104] JS：防抖
来源：http://hz.cucudq.cn/gtpacjtysg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtvpgaabao.html

[U105] JS：节流
来源：http://hz.zhaomingkeji.xyz/gtwuvnruqm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shuidangran.top/gtiisvzsmy.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtmnpjjgal.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.pengpengdd.cyou/gtugduhiyb.html

[U107] JS：数字千分位
来源：http://hz.bjfxy.top/gtvdtflqjk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnqzz.top/gtzcbfsvol.html

[U108] JS：随机整数
来源：http://hz.redwolf501.top/gtcwqqcxso.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangtech.top/gtnkdvwstq.html

[U109] JS：数组分组
来源：http://hz.nwbrower.top/gtvgxwpkct.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gteixwrwsd.html

[U110] JS：数组分块
来源：http://hz.xziqi.cn/gtxsdmygsb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.aibaodan.cn/gtqohnyixv.html

[U111] JS：对象转 Map
来源：http://hz.aizwys.cn/gtugwuwise.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtlnytcwxk.html

[U112] JS：字符串补位
来源：http://hz.ydzc1.top/gtqueoedgb.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtfpgddune.html

[U113] JS：正则替换全部
来源：http://hz.jinghuilouyu.cn/gtttgbingn.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtrpwznjga.html

[U114] JS：JSON 深比较
来源：http://hz.snrcjt.cn/gtwhocgorl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtqgcbmlhx.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtbyayoftz.html

crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtnhahggjs.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shzxlz.cn/gtksrgtbbq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtdplwpejb.html

[U117] JS：单元测试
来源：http://hz.zhongyouzk.top/gtyzwkaadw.html

npm i -D vitest;  npx vitest
来源：http://hz.shuidangran.top/gtqducyjdq.html

[U118] JS：开发服务器
来源：http://hz.yueranfly.top/gtoencvdti.html

npm i -D vite;  npx vite
来源：http://hz.jlsjyb.cn/gtosowffdp.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtnfljehkr.html

npx vite build
来源：http://hz.sweek.top/gtmpjfyvxn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hammf.cn/gtrffwofsr.html

import.meta.env.VITE_API_URL
来源：http://hz.cashguo.top/gthprsockh.html

================================================================================
来源：http://hz.xinyue.icu/gtyvohmonl.html

统计汇总
来源：http://hz.aizwys.cn/gtimffegia.html

================================================================================
来源：http://hz.jinqigufen.top/gtiyhdujnl.html

按语言统计（条）：
来源：http://hz.tanke756.top/gtktbcblxt.html

Python ......... 252
来源：http://hz.yvedp.cn/gtmosylrlv.html

PHP ............ 252
来源：http://hz.hnqzz.top/gtcehzvsjw.html

JavaScript ..... 252
来源：http://hz.jinqigfzy.top/gtwixpiypk.html

TypeScript ..... 212
来源：http://hz.snrcjt.cn/gtxavkjlkd.html

Java ........... 212
来源：http://hz.aizwys.cn/gtfeaudsct.html

Go ............. 212
来源：http://hz.jqgfzy.top/gtlfijbihc.html

Ruby ........... 212
来源：http://hz.meibo888.top/gtxvoiebji.html

C# ............. 212
来源：http://hz.nanxinkj.top/gtghlbreni.html

C .............. 30
来源：http://hz.sufxvd.cn/gtrbqvqrbe.html

C++ ............ 30
来源：http://hz.wangshuangyany.cn/gtwbdvtupu.html

SQL ............ 90
来源：http://hz.gogol.net.cn/gtxtrlevls.html

Bash ........... 80
来源：http://hz.aibaodan.cn/gttrlbeejr.html

Kotlin ......... 15
来源：http://hz.dashuyun.cn/gtzrhehoef.html

Swift .......... 15
来源：http://hz.yj20258.top/gtghzsdvje.html

Lua ............ 10
来源：http://hz.nwbrower.top/gtgghiaelm.html

Perl ........... 10
来源：http://hz.redwolf501.top/gtjwwsmjlu.html

Scala .......... 10
来源：http://hz.jinqigufen.top/gtmtfsjrkx.html

------------------------------------
来源：http://hz.yuxming.cn/gtjetzmzba.html

合计 ........... 2106 条
来源：http://hz.dashuyun.cn/gtfjyphahw.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtemvawrio.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenlongwang.top/gtykxutdyq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtuuoqqqrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtygtamyit.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtzwwudhvb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cashguo.top/gtehxiedba.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtchduqrjg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtkqfnfbho.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtfvxoneah.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtfnkgtxnl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtkznjzmeq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtzvzzddxo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtnkgaozns.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtqgtzygjn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtuciksvbs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258888.top/gtpzuljjrh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtfznbzntr.html

Q SQL 专题                              90
来源：http://hz.bjfxy.top/gtbzarrhfi.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtcuteuavz.html

S C / C++ 专题                          60
来源：http://hz.ppjwa.cn/gtojmojods.html

T 其他语言补充                          60
来源：http://hz.xylfe.cn/gtfgypkmka.html

U 高频实用片段                         120
来源：http://hz.hnqzz.top/gtojcfkoax.html

------------------------------------
来源：http://hz.cashguo.top/gtzskgsjix.html

合计                                  2106 条
来源：http://hz.hongshengwenyu.top/gtqsmbcjru.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtwunvtjdl.html

使用提醒
来源：http://hz.cdnleiting.top/gtfatrakam.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtnywhjecy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yonumen.top/gtivbueowk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yonumen.top/gtzydryvbn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gtmuwmajvz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.bjfxy.top/gtndcluagh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.svipenyu.cn/gtuectzyie.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtxujpitfm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqthggnld.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.pengpengdd.cyou/gtaufotbss.html

Common Programming Examples Cheat Book
来源：http://hz.yongpay.top/gtagsrtfip.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjenyiryq.html

【收录内容】
来源：http://hz.zhijiandao.cn/gtburoayqc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sufxvd.cn/gttffoeqww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.meibo888.top/gtjimyuhny.html

SQL · Bash · C · C++
来源：http://hz.nanxinkj.top/gtpvivktbj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.0kj1m.cn/gtyeozpchi.html

【使用说明】
来源：http://hz.yj202588.top/gtjwufordb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gtzxfhtdei.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydzc1.top/gtxjghndht.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hfpthk.cn/gtmsfsprar.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.fzhhl.top/gtyoeqdpta.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.tian-w.cn/gtopuhjwnv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtbckjatxd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ybcxt.top/gtoadugxcl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cheryme.top/gtixluffge.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shuidangran.top/gttpiwyqvf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.guannengcc.top/gtwbbmysem.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.0kj1m.cn/gttzygxrow.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yvedp.cn/gtlehgejmv.html

【文件统计】
来源：http://hz.c1oappe.top/gtodotrkuc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yueranfly.top/gtxslfwvaf.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtkhghtyzt.html

目  录
来源：http://hz.shangyingyoupin.top/gtudyokhpm.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gthdgnqiha.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gtwhpteztr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gttuitipzb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtqqsqnswh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtodgtrwll.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hammf.cn/gtgkuukrmy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gttlhfdzfo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cheryme.top/gttffbnucm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.wangdashe.top/gtmynqaipv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jlsjyb.cn/gtifyzthxa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gteinyjsrl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtqhluvuml.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtqjaqwpcs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtlckfmsbl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.mhx1999.top/gtznwxedhv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cashguo.top/gtdkmcmxxh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtuhzuvqen.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shanyushiyangkeji.top/gtqkldqdcd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nanxuanxn.top/gtqjkeldvw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hammf.cn/gtfywbqmco.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtrbmoebkc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gthllcvpzf.html

================================================================================
来源：http://hz.tian-w.cn/gtuiiyrdmw.html

A. 基础语法与类型
来源：http://hz.cdnleiting.top/gtcjofjift.html

================================================================================
来源：http://hz.cucudq.cn/gtzeytaeyl.html

[A01] Hello World
来源：http://hz.xingfuxueyuan.xyz/gtatjhaccp.html

Py:   print("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtcdlgabfk.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtgskxaeci.html

JS:   console.log("Hello, World!");
来源：http://hz.xuetiantiany.cn/gtoeymylfm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.iojbl.cn/gtbjrkkaok.html

Java: System.out.println("Hello, World!");
来源：http://hz.zycfv.cn/gtvkilfzro.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xingfuxueyuan.xyz/gtwpncuajo.html

Ruby: puts "Hello, World!"
来源：http://hz.yongpay.top/gtcnjkoemf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuxming.cn/gtomwhpiks.html

[A02] 变量声明与赋值
来源：http://hz.svipenyu.cn/gtfedblrsj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tian-w.cn/gttyujdzyx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fengsongda.top/gtoomohjfp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.nanxinkj.top/gtmyiewtdl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.dianchejie.cn/gtwbiysvke.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhijiandao.cn/gtbolqhpsd.html

Go:   name := "Alex"; age := 20
来源：http://hz.shanyushiyangkeji.top/gtnxwqjksl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtayenvmok.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtuoxgifbg.html

[A03] 常量定义
来源：http://hz.redwolf501.top/gtdpkgxszm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhongyouzk.top/gtmvxhmrgh.html

PHP:  const PI = 3.14159;
来源：http://hz.smart0.xyz/gtvsuwxkql.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gtygrmkndq.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtgctarziz.html

Java: static final double PI = 3.14159;
来源：http://hz.meibo888.top/gtmbinyozp.html

Go:   const PI = 3.14159
来源：http://hz.xziqi.cn/gtljlqbloz.html

Ruby: PI = 3.14159
来源：http://hz.yonumen.top/gtxbzlinfv.html

C#:   const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtrrmxlygh.html

[A04] 判断变量类型
来源：http://hz.yangfankeji.com/gtxhbuzjpe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.daria6918.cn/gtvfkoevqa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.cqqwz.cn/gtqdxacxig.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aizwys.cn/gtfpedveqw.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gttshpakbc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.tanke756.top/gtkwgpdmxd.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tanke756.top/gtpdoyflwk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.mhx1999.top/gtlfpdjort.html

C#:   x.GetType().Name; x is int
来源：http://hz.pycfn.com/gthtwrpwht.html

[A05] 整数除法与取模
来源：http://hz.cdnleiting.top/gtafaighov.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hfpthk.cn/gthrvnplmw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxuanxn.top/gtlooiyofo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtfmrrvfzf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtjwhahyhb.html

Java: 7 / 2; 7 % 2
来源：http://hz.iojbl.cn/gtfyokptxs.html

Go:   7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtquqjbvmp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ivvv.top/gtwnriecca.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtzhtfzfte.html

[A06] 字符串转数字
来源：http://hz.snrcjt.cn/gtrapdgcun.html

Py:   int("42"); float("3.14")
来源：http://hz.gogol.net.cn/gteeypvesa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cheryme.top/gthekiqgtx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ehwqpu.com/gtjnsrkunw.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guowangkeji.top/gtkmnexdfi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.dashuyun.cn/gtkyjqvcxs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhengqikj.top/gtfcartynr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sysykeji.top/gtbeblborm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hnxiangtu.top/gtkblzzwqz.html

[A07] 数字转字符串
来源：http://hz.yj202588.top/gtqzkmyrir.html

Py:   str(42)
来源：http://hz.jlsjyb.cn/gtmyjnjamz.html

PHP:  (string) 42; strval(42)
来源：http://hz.aibaodan.cn/gtfabzuztg.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258.top/gtfaizekwz.html

TS:   String(42)
来源：http://hz.cashguo.top/gtmrvgeihx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.feifeiyinyue.top/gtytooubde.html

Go:   strconv.Itoa(42)
来源：http://hz.birdmap.top/gtwwrnpxpz.html

Ruby: 42.to_s
来源：http://hz.zdqjudy.top/gtoxwbpavm.html

C#:   42.ToString()
来源：http://hz.hongshengwenyu.top/gtdhipablw.html

[A08] 取整与四舍五入
来源：http://hz.mhx1999.top/gtedanhwri.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ydjk.org.cn/gtwnpoblnx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.c1oappe.top/gtrrtoupxl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.birdmap.top/gtfbgojzzu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ydzc1.top/gtphkwfohv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ydjk.org.cn/gtabdofirg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.daria6918.cn/gtkluhekrh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xziqi.cn/gtoozjozkp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.chenlongwang.top/gtkveygdfc.html

[A09] 绝对值与最大最小值
来源：http://hz.sysykeji.top/gtdlcovdxl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.9152youxi.cn/gtzpnvjwlc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj202588.top/gthwftjikj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yueranfly.top/gtybpbntuf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jiagoushi.top/gtyiifflca.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.andypj.xyz/gtxndpepsw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jlsjyb.cn/gtotnzgbcf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hfpthk.cn/gtxofajnca.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.haohaochexian.top/gtpadcxqkb.html

[A10] 生成随机数
来源：http://hz.nwbrower.top/gtpizvuitv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xuetiantiany.cn/gtlvdaonjo.html

PHP:  random_int(1, 100);
来源：http://hz.shangyingyoupin.top/gthycffjij.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cucudq.cn/gtysyhzwgy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zdqjudy.top/gtrgohjuqj.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yuanzhike.top/gtkximznqd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.dianchejie.cn/gtleialptd.html

Ruby: rand(1..100)
来源：http://hz.dashuyun.cn/gtqbaginxf.html

C#:   new Random().Next(1, 101)
来源：http://hz.hfpthk.cn/gtrjckzrch.html

[A11] 条件表达式（三元）
来源：http://hz.jinqigufen.top/gtkwmvxxgs.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.mhx1999.top/gtirnqjwzn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.nanxuanxn.top/gtbjjqsesq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jyoumei.cn/gtfjipjhkp.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.tanke756.top/gtqtoiacsi.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtsgmatsii.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.birdmap.top/gtcvtkkxmq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtgnmlxabn.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xuanzx.com/gtpntshirt.html

[A12] 字符串插值 / 格式化
来源：http://hz.pycfn.com/gtlsepjctd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.zhaomingkeji.xyz/gtfzrmhmoz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jyoumei.cn/gtyopqtjrg.html

JS:   `Hello, ${name}!`
来源：http://hz.52xcode.cn/gtesvklnuk.html

TS:   `Hello, ${name}!`
来源：http://hz.hfpthk.cn/gtwnjkirtm.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.havefunace.top/gtvhbbjclm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yonumen.top/gtnzpstmrp.html

Ruby: "Hello, #{name}!"
来源：http://hz.yj202588.top/gtcjcpoabo.html

C#:   $"Hello, {name}!"
来源：http://hz.zhaomingkeji.xyz/gtyedpcigz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yueranfly.top/gturxgeneh.html

Py:   "第一行\n第二行"
来源：http://hz.yvedp.cn/gtwpjzdocp.html

PHP:  "第一行\n第二行"
来源：http://hz.aizwys.cn/gtgfwpxnqo.html

JS:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtiylvuahd.html

TS:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtfbvzgrpw.html

Java: "第一行\n第二行"
来源：http://hz.cashguo.top/gtlpawjmjx.html

Go:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtumyeqpfg.html

Ruby: "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtzchaprrw.html

C#:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtnnlshzcg.html

[A14] 注释写法
来源：http://hz.zdqjudy.top/gtvytsnfni.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhongyouzk.top/gteuwjpidq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.daxiang520.top/gteymjzfqa.html

JS:   // 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gtmnbrrhmn.html

TS:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gthcitbymu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.ydjk.org.cn/gtzuetqefs.html

Go:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gtdjgkqudn.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jianghu66.top/gtscldsdsa.html


<!-- 参考信息 -->