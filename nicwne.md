代发 wailian999

[U89] JS：数组去重
来源：http://hz.ydjk.org.cn/gtgygjmzzv.html

[...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtdgeamgls.html

[U90] JS：数字数组排序
来源：http://hz.vqdsnc.cn/gtqpvxkojh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gttmuthakm.html

[U91] JS：对象键值遍历
来源：http://hz.nanxinkj.top/gtqpirtxge.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jqgfzy.top/gtukbbuqzr.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtispwvcaj.html

structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtygbucqiq.html

[U93] JS：模板字符串
来源：http://hz.wangshuangyany.cn/gtvodbuqiw.html

`共 ${n} 条`
来源：http://hz.smart0.xyz/gtggvkcbjn.html

[U94] JS：箭头函数
来源：http://hz.yongpay.top/gtiikwwunx.html

const double = x => x * 2;
来源：http://hz.52xcode.cn/gtqvpdkesy.html

[U95] JS：Promise 包装
来源：http://hz.sufxvd.cn/gtkarfgdvn.html

new Promise((resolve, reject) => {})
来源：http://hz.nwbrower.top/gtqulqdicu.html

[U96] JS：async/await 与异常
来源：http://hz.svipenyu.cn/gtsqfuijux.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydzc1.top/gttwdpvoqk.html

[U97] JS：并发请求
来源：http://hz.yuxming.cn/gtkcdjmvpy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gthmyisqww.html

[U98] JS：fetch 带 JSON
来源：http://hz.iojbl.cn/gtsbqswvcx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hfpthk.cn/gtrstwjhak.html

[U99] JS：事件监听
来源：http://hz.ydjk.org.cn/gtfoqvkxpu.html

el.addEventListener("click", e => {})
来源：http://hz.chenjidiqi.icu/gtriutcqlz.html

[U100] JS：DOM 查询
来源：http://hz.ivvv.top/gtkgzyejfg.html

document.querySelector(".item")
来源：http://hz.jinyuanbaomall.cn/gtfxpdbjmn.html

[U101] JS：classList 操作
来源：http://hz.sxryk.cn/gtnbpvebpp.html

el.classList.toggle("active")
来源：http://hz.ydzc1.top/gtkoguxkmv.html

[U102] JS：本地存储
来源：http://hz.shzxlz.cn/gtdawuydyq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guannengcc.top/gtgijsrtdk.html

[U103] JS：定时器
来源：http://hz.chenlongwang.top/gtmyfrpfkz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gthwobglwl.html

[U104] JS：防抖
来源：http://hz.feifeiyinyue.top/gtjyqjmxth.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtuylhwlrn.html

[U105] JS：节流
来源：http://hz.yangfankeji.com/gtjfhxftwe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258.top/gthurgbqtk.html

[U106] JS：日期格式化
来源：http://hz.xinyue.icu/gtpcknnpue.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cashguo.top/gtevmdhcqa.html

[U107] JS：数字千分位
来源：http://hz.jyoumei.cn/gtkwewyljb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xziqi.cn/gtziqddhig.html

[U108] JS：随机整数
来源：http://hz.vqdsnc.cn/gtwknaszbb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cucudq.cn/gtyrbktjnt.html

[U109] JS：数组分组
来源：http://hz.bjfxy.top/gtweyhlsfb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtpayqwxbk.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtcrhbppda.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigfzy.top/gtnzeznvyy.html

[U111] JS：对象转 Map
来源：http://hz.svipenyu.cn/gthvocqxxk.html

new Map(Object.entries(obj))
来源：http://hz.gotoacloud.top/gtignevijy.html

[U112] JS：字符串补位
来源：http://hz.dashuyun.cn/gtfipdqrxr.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtkcmeqbvv.html

[U113] JS：正则替换全部
来源：http://hz.yj202588.top/gtcpkayfqz.html

s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtrizyudsy.html

[U114] JS：JSON 深比较
来源：http://hz.fengsongda.top/gtqyudipue.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtkcpceeuv.html

[U115] JS：生成 UUID
来源：http://hz.gogol.net.cn/gtpcehrlas.html

crypto.randomUUID()
来源：http://hz.daxiang520.top/gtnwzuvogb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ybcxt.top/gthfprliim.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hongshengwenyu.top/gtabaxzupe.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gtmjaschto.html

npm i -D vitest;  npx vitest
来源：http://hz.aibaodan.cn/gtlqpdhiyu.html

[U118] JS：开发服务器
来源：http://hz.ydjk.org.cn/gtdufnhkci.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtktkoguql.html

[U119] JS：生产构建
来源：http://hz.xingfuxueyuan.xyz/gtnkyyzfbg.html

npx vite build
来源：http://hz.yanxiufei.cn/gthuviruzq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydzc1.top/gtgsfsaxar.html

import.meta.env.VITE_API_URL
来源：http://hz.havefunace.top/gtbmaidnxp.html

================================================================================
来源：http://hz.shzxlz.cn/gtoxgntyti.html

统计汇总
来源：http://hz.zhiwuduotai.top/gtlqjhrdvw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnpkvvfun.html

按语言统计（条）：
来源：http://hz.sysykeji.top/gtyqgadfum.html

Python ......... 252
来源：http://hz.jinqigufen.top/gtsuiejelg.html

PHP ............ 252
来源：http://hz.zdqjudy.top/gtubpwjxnv.html

JavaScript ..... 252
来源：http://hz.zhoulong.xyz/gtfhcrzzgg.html

TypeScript ..... 212
来源：http://hz.gzhubu.top/gtuutbbnct.html

Java ........... 212
来源：http://hz.shanyushiyangtech.top/gtvmhybzlg.html

Go ............. 212
来源：http://hz.daria6918.cn/gtyjaxsflz.html

Ruby ........... 212
来源：http://hz.gzhubu.top/gthjwuisoq.html

C# ............. 212
来源：http://hz.feifeiyinyue.top/gtesgdjefh.html

C .............. 30
来源：http://hz.jyoumei.cn/gtnyrnchre.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtvattevhv.html

SQL ............ 90
来源：http://hz.wangdashe.top/gtmznvccar.html

Bash ........... 80
来源：http://hz.ivvv.top/gtyplonfvc.html

Kotlin ......... 15
来源：http://hz.c1oappe.top/gtpuvsmjwz.html

Swift .......... 15
来源：http://hz.zhengqikj.top/gtswmpyruh.html

Lua ............ 10
来源：http://hz.kuanghao11.cn/gtfkpgbguh.html

Perl ........... 10
来源：http://hz.xziqi.cn/gtptqzbogt.html

Scala .......... 10
来源：http://hz.ivvv.top/gtilczedtn.html

------------------------------------
来源：http://hz.snrcjt.cn/gtgcoieydl.html

合计 ........... 2106 条
来源：http://hz.hfpthk.cn/gtpxlkrwvc.html

按章节统计：
来源：http://hz.pycfn.com/gtcgymirzz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtjcqmbhid.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtfpjrrica.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtqbvtvikr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtirdamtbl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guowangkeji.top/gtagwrekup.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.meibo888.top/gtefdvxngj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ydzc1.top/gtkwtvbmks.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtscopukne.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtdmbqicou.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gteyrkzphc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtecboqbrd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtkhiauhzz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtzzbmcppe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.9152youxi.cn/gthwspyiih.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgfzy.top/gtxgiczukt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtthddwnnz.html

Q SQL 专题                              90
来源：http://hz.ydjk.org.cn/gtpzjlkesc.html

R Bash 专题                             80
来源：http://hz.zhixingplan.top/gtjnphyqhd.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangkeji.top/gtufxijadm.html

T 其他语言补充                          60
来源：http://hz.cashguo.top/gtwrdwbgtm.html

U 高频实用片段                         120
来源：http://hz.sxryk.cn/gtppkjkcjm.html

------------------------------------
来源：http://hz.yonumen.top/gtyejynqgt.html

合计                                  2106 条
来源：http://hz.jiagoushi.top/gtjeeuchxb.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtbsudpkzz.html

使用提醒
来源：http://hz.ywan-chungtsiang.top/gtvlkqgrql.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtkzlaurpb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ehwqpu.com/gtarbzznkw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.feifeiyinyue.top/gtobrghcod.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenzaomai.com/gtwjhlimgu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtdureudho.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zdqjudy.top/gtykredxhl.html

—— 文件结束 ——
来源：http://hz.guannengcc.top/gtoymjgeyh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtazxqhzeu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zdqjudy.top/gtepkqmyrg.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigufen.top/gtgkrwuedy.html

================================================================================
来源：http://hz.gotoacloud.top/gtddebllrh.html

【收录内容】
来源：http://hz.meibo888.top/gtcrtzcvcq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhaomingkeji.xyz/gtaqkhyayb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.andypj.xyz/gtgsoqqwkc.html

SQL · Bash · C · C++
来源：http://hz.hnxiangtu.top/gteoivzabe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.smart0.xyz/gtnifgumnh.html

【使用说明】
来源：http://hz.jinyuanbaomall.cn/gtkfvoiqoi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenzaomai.com/gtuaoyzfti.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.havefunace.top/gtdcrjrpdd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ivvv.top/gtshlvruhr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtsxtnhjon.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jianghu66.top/gtksrsxvcm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.andypj.xyz/gtjtlytdtn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haohaochexian.top/gtsbanfken.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinghuilouyu.cn/gtytcmmuej.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtuctlemgd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj202588.top/gtdibjxktm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sufxvd.cn/gthnwzupfd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zycfv.cn/gtnllggewe.html

【文件统计】
来源：http://hz.gzhubu.top/gttgpibqvc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtjqqrrqbv.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtlophdjat.html

目  录
来源：http://hz.shanyushiyangkeji.top/gtekvhwaev.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtvadgwnpx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dashuyun.cn/gtfsqxchnn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtkqicwwep.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gtujyfgnsx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtzgxvebpt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xuanzx.com/gttloywijw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yueranfly.top/gttpgouwlf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gtksyvamga.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hfpthk.cn/gtswufdsaf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtkousrhmx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jlsjyb.cn/gtyxmngqqf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtriwfrmqg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtwizhztey.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtcdtjnyxe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtqawsqbjp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhijiandao.cn/gtmcbiflra.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtipybgtfe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.dashuyun.cn/gtmuwvemnu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.haohaochexian.top/gtlxiwdkew.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gtndciduyg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtzpsvbtop.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.vqdsnc.cn/gtjopdwafq.html

================================================================================
来源：http://hz.chenzaomai.com/gthpkpsbzk.html

A. 基础语法与类型
来源：http://hz.xuetiantiany.cn/gtzwtezmnt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthxoxdtpa.html

[A01] Hello World
来源：http://hz.daria6918.cn/gtauglbfuc.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtspdtrtmh.html

PHP:  echo "Hello, World!";
来源：http://hz.shuidangran.top/gtzekzfjjb.html

JS:   console.log("Hello, World!");
来源：http://hz.vqdsnc.cn/gtuyydgnkt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tanke756.top/gtoaywuunb.html

Java: System.out.println("Hello, World!");
来源：http://hz.yueranfly.top/gthwqvmsld.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenzaomai.com/gthmynzmbs.html

Ruby: puts "Hello, World!"
来源：http://hz.jinghuilouyu.cn/gtpcbstqwi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtknuxjpdj.html

[A02] 变量声明与赋值
来源：http://hz.yj202588.top/gtnkaosqft.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gotoacloud.top/gtwkjvnfkv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gttqtmuvsj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuanzx.com/gtvrvfmchq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.smart0.xyz/gtytodfsfu.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gthushwevh.html

Go:   name := "Alex"; age := 20
来源：http://hz.yongpay.top/gtwzdglqsw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.birdmap.top/gtfblllbnb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtagfianlk.html

[A03] 常量定义
来源：http://hz.ehwqpu.com/gtptcybutd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hammf.cn/gtlcbamwdm.html

PHP:  const PI = 3.14159;
来源：http://hz.c1oappe.top/gtddslvbgx.html

JS:   const PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtrhzrdmli.html

TS:   const PI: number = 3.14159;
来源：http://hz.aizwys.cn/gtcpkrnpmx.html

Java: static final double PI = 3.14159;
来源：http://hz.cheryme.top/gtyuludctd.html

Go:   const PI = 3.14159
来源：http://hz.sysykeji.top/gtfmuagsmn.html

Ruby: PI = 3.14159
来源：http://hz.zhoulong.xyz/gtnbhieutr.html

C#:   const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtczmezryx.html

[A04] 判断变量类型
来源：http://hz.gotoacloud.top/gtbhdmfcne.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.dianchejie.cn/gtvdcqcfrt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.c1oappe.top/gtgexcdqdf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.svipenyu.cn/gtdpbanrch.html

TS:   typeof x; x instanceof Date
来源：http://hz.andypj.xyz/gtyxkhselu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xingfuxueyuan.xyz/gtgdmgigdj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhaomingkeji.xyz/gtwlilqzfe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shzxlz.cn/gtkcygpzrf.html

C#:   x.GetType().Name; x is int
来源：http://hz.ydjk.org.cn/gtgnumkwhv.html

[A05] 整数除法与取模
来源：http://hz.chenjidiqi.icu/gtfhbcdqth.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nwbrower.top/gtapcfbdes.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhixingplan.top/gtqpogsfop.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.dianchejie.cn/gtwmewpxjb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sysykeji.top/gtatdaapot.html

Java: 7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gturbcgjrd.html

Go:   7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtjkqfesyd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtyavhbklr.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuxming.cn/gtopifyqml.html

[A06] 字符串转数字
来源：http://hz.c1oappe.top/gtwjvlcdia.html

Py:   int("42"); float("3.14")
来源：http://hz.chenjidiqi.icu/gthgahbjsh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinyuanbaomall.cn/gtyzggewdm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hysaishi.cn/gtxxfpxeme.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jianghu66.top/gtvmsqiifb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sysykeji.top/gtlshbgxft.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.havefunace.top/gtoqvakvrh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hnxiangtu.top/gthqsrmsou.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinghuilouyu.cn/gtmvkkqdod.html

[A07] 数字转字符串
来源：http://hz.ppjwa.cn/gtsukkpvkm.html

Py:   str(42)
来源：http://hz.yangfankeji.com/gtyrfxyhrc.html

PHP:  (string) 42; strval(42)
来源：http://hz.daxiang520.top/gtpwzzazzy.html

JS:   String(42); (42).toString()
来源：http://hz.hysaishi.cn/gtdehhloug.html

TS:   String(42)
来源：http://hz.ywan-chungtsiang.top/gtybxjkwca.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.316326.xyz/gtjnpyjdwx.html

Go:   strconv.Itoa(42)
来源：http://hz.gaohongyu789.top/gtsfgiumkn.html

Ruby: 42.to_s
来源：http://hz.9152youxi.cn/gtxlpygece.html

C#:   42.ToString()
来源：http://hz.52xcode.cn/gtdnhyivun.html

[A08] 取整与四舍五入
来源：http://hz.jinyuanbaomall.cn/gtctoetqxb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.tian-w.cn/gthunbnfhm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.smart0.xyz/gtanwazfed.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtppthfomq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ybcxt.top/gtunfxqown.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtfikctmcc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hnxiangtu.top/gtsszwldxg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.smart0.xyz/gtekiqyzqj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.havefunace.top/gtwrhsffme.html

[A09] 绝对值与最大最小值
来源：http://hz.dashuyun.cn/gtmsqczyun.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xziqi.cn/gtmlmgdusz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtlvxsvttk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.kuanghao11.cn/gtlunapzoi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtdusudost.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtvremwkaw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.dianchejie.cn/gtbrkeyibx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cucudq.cn/gtfthapfdn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtbyyyaayn.html

[A10] 生成随机数
来源：http://hz.hnqzz.top/gtrywzlrjz.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yj202588.top/gtmezebwno.html

PHP:  random_int(1, 100);
来源：http://hz.wangshuangyany.cn/gtdfovzgyf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigufen.top/gtsdalocbk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.tian-w.cn/gtmgasliiu.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cdnleiting.top/gtizfhgdzu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.nanxinkj.top/gtjhwaewtj.html

Ruby: rand(1..100)
来源：http://hz.yangfankeji.com/gtflmvzawb.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj20258.top/gtsyxzppqk.html

[A11] 条件表达式（三元）
来源：http://hz.zhaomingkeji.xyz/gtrmoiypfi.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hnqzz.top/gtopeeguyy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtyyfchqvh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtlpjpnfns.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtkfrbytum.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtvsdtrpma.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xylfe.cn/gtfijsbufx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtihdicmig.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.birdmap.top/gtrukbrgfv.html

[A12] 字符串插值 / 格式化
来源：http://hz.sufxvd.cn/gtvmcywnwy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.ywan-chungtsiang.top/gtmkuhhjuf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jiagoushi.top/gtgcchgfqx.html

JS:   `Hello, ${name}!`
来源：http://hz.wangshuangyany.cn/gtfwxoaltw.html

TS:   `Hello, ${name}!`
来源：http://hz.nanxinkj.top/gtrcybrrgo.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hywenlv.cn/gttmreedtb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hongshengwenyu.top/gtyhjikfjq.html

Ruby: "Hello, #{name}!"
来源：http://hz.zhoulong.xyz/gtcpqaorhn.html

C#:   $"Hello, {name}!"
来源：http://hz.9152youxi.cn/gtdljfaekd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hnxiangtu.top/gtkenbhrwv.html

Py:   "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtbcisaffq.html

PHP:  "第一行\n第二行"
来源：http://hz.sysykeji.top/gtkfcovqjk.html

JS:   "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtgxehecef.html

TS:   "第一行\n第二行"
来源：http://hz.nanxuanxn.top/gteyhzlnyn.html

Java: "第一行\n第二行"
来源：http://hz.sysykeji.top/gtjclbiaol.html

Go:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtrckuttwk.html

Ruby: "第一行\n第二行"
来源：http://hz.jqgufenzy.top/gtxirlvysx.html

C#:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtnspcwpiu.html

[A14] 注释写法
来源：http://hz.zhijiandao.cn/gtbbtvfpbe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.xingfuxueyuan.xyz/gtcagiqfzo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtkntzwhme.html

JS:   // 单行；/* 多行 */
来源：http://hz.yuxming.cn/gtdrfrkpac.html

TS:   // 单行；/* 多行 */
来源：http://hz.jianghu66.top/gtsicixzih.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jianghu66.top/gtlhurovht.html

Go:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtrklqdyci.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.dianchejie.cn/gtmezzutje.html

C#:   // 单行；/* 多行 */
来源：http://hz.hywenlv.cn/gtrmrmginw.html

[A15] 空值判断与默认值
来源：http://hz.52xcode.cn/gtdyqiuyfm.html

Py:   value = data or "默认值"
来源：http://hz.xingfuxueyuan.xyz/gtdlbgfamr.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.dianchejie.cn/gtwrydmtpu.html


<!-- 参考信息 -->