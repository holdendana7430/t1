代发 wailian999

[U89] JS：数组去重
来源：http://hz.fengsongda.top/gtzyqsglgh.html

[...new Set(arr)]
来源：http://hz.aibaodan.cn/gthfdeudyv.html

[U90] JS：数字数组排序
来源：http://hz.zhoulong.xyz/gtxyojfmjq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtwukstrvk.html

[U91] JS：对象键值遍历
来源：http://hz.zhengqikj.top/gtnfhdnxyf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yueranfly.top/gtiqtphktb.html

[U92] JS：深拷贝
来源：http://hz.aizwys.cn/gtgejokmac.html

structuredClone(obj)
来源：http://hz.daxiang520.top/gtnuxhmchn.html

[U93] JS：模板字符串
来源：http://hz.gotoacloud.top/gtmdevccvd.html

`共 ${n} 条`
来源：http://hz.cqqwz.cn/gtewezwkiz.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gtekarhktn.html

const double = x => x * 2;
来源：http://hz.hammf.cn/gtyobtnpmp.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtqeewbxpo.html

new Promise((resolve, reject) => {})
来源：http://hz.ehwqpu.com/gtzfuzmeth.html

[U96] JS：async/await 与异常
来源：http://hz.haohaochexian.top/gtwaotpads.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtffmudzlu.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtcrkxuizi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtseshbzcu.html

[U98] JS：fetch 带 JSON
来源：http://hz.bjfxy.top/gtteodygle.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daxiang520.top/gtakqzzjqi.html

[U99] JS：事件监听
来源：http://hz.jianghu66.top/gthzzogfzs.html

el.addEventListener("click", e => {})
来源：http://hz.xuetiantiany.cn/gtpqvdfhmv.html

[U100] JS：DOM 查询
来源：http://hz.yj20258888.top/gtiebkrphn.html

document.querySelector(".item")
来源：http://hz.gotoacloud.top/gtqlrzifoi.html

[U101] JS：classList 操作
来源：http://hz.pycfn.com/gtzqymagih.html

el.classList.toggle("active")
来源：http://hz.jiagoushi.top/gtryivjvbw.html

[U102] JS：本地存储
来源：http://hz.jinyuanbaomall.cn/gtkwuchlwy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yonumen.top/gtmjqwfike.html

[U103] JS：定时器
来源：http://hz.andypj.xyz/gtnkgsfpcg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangkeji.top/gtlmujvskf.html

[U104] JS：防抖
来源：http://hz.xinyue.icu/gtxmxkyxir.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtepgxstth.html

[U105] JS：节流
来源：http://hz.zhengqikj.top/gtgkevzzhh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhijiandao.cn/gtuwirhovr.html

[U106] JS：日期格式化
来源：http://hz.nanxuanxn.top/gtumqtaguu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenjidiqi.icu/gtrwgcvlcv.html

[U107] JS：数字千分位
来源：http://hz.zycfv.cn/gtmixfdwen.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.iojbl.cn/gtgrhjzisa.html

[U108] JS：随机整数
来源：http://hz.jinqigufen.top/gtwrhsyswk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fengsongda.top/gtdwupzfxs.html

[U109] JS：数组分组
来源：http://hz.smart0.xyz/gtmciuvvgc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtgkzqungt.html

[U110] JS：数组分块
来源：http://hz.jinyuanbaomall.cn/gtsuwexlhi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.birdmap.top/gtpnetosyr.html

[U111] JS：对象转 Map
来源：http://hz.bjfxy.top/gtmiovetbw.html

new Map(Object.entries(obj))
来源：http://hz.9152youxi.cn/gtjxrdelcm.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtwgqfehoc.html

"7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtslusxnqp.html

[U113] JS：正则替换全部
来源：http://hz.pengpengdd.cyou/gtiifzzgbk.html

s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtifmthsxp.html

[U114] JS：JSON 深比较
来源：http://hz.shanyushiyangkeji.top/gtcywnvahv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtenzvdlmr.html

[U115] JS：生成 UUID
来源：http://hz.dianchejie.cn/gthbeztwuo.html

crypto.randomUUID()
来源：http://hz.xylfe.cn/gtmnmhkucz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xziqi.cn/gtowaopbsp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ppjwa.cn/gtesoiwklv.html

[U117] JS：单元测试
来源：http://hz.havefunace.top/gthtdqdkdu.html

npm i -D vitest;  npx vitest
来源：http://hz.cqqwz.cn/gtwanotdbr.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtdbygbwbv.html

npm i -D vite;  npx vite
来源：http://hz.yonumen.top/gtrcscqysk.html

[U119] JS：生产构建
来源：http://hz.pycfn.com/gtqewwtmtt.html

npx vite build
来源：http://hz.ybcxt.top/gtsruefvhl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258.top/gtgwcnvzsf.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258.top/gtplanmirz.html

================================================================================
来源：http://hz.hammf.cn/gtyldgrrxl.html

统计汇总
来源：http://hz.andypj.xyz/gtqvyiwlmp.html

================================================================================
来源：http://hz.gzhubu.top/gtdbvbqduf.html

按语言统计（条）：
来源：http://hz.zhijiandao.cn/gtukuqzvkx.html

Python ......... 252
来源：http://hz.xingfuxueyuan.xyz/gtnxmwvvig.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtpgeoyusg.html

JavaScript ..... 252
来源：http://hz.yj20258888.top/gttcigonez.html

TypeScript ..... 212
来源：http://hz.hnqzz.top/gtuaofhgou.html

Java ........... 212
来源：http://hz.zhaomingkeji.xyz/gtobrqsikr.html

Go ............. 212
来源：http://hz.0kj1m.cn/gtenwwyfyr.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtmvilbtay.html

C# ............. 212
来源：http://hz.jiagoushi.top/gtsztlfsdq.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtlrtsqzuk.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtiyrgezlx.html

SQL ............ 90
来源：http://hz.hnqzz.top/gttfskveex.html

Bash ........... 80
来源：http://hz.jiagoushi.top/gtwbzbdxpl.html

Kotlin ......... 15
来源：http://hz.sufxvd.cn/gthsefgqmx.html

Swift .......... 15
来源：http://hz.shangyingyoupin.top/gthhllnvig.html

Lua ............ 10
来源：http://hz.zhiwuduotai.top/gtllszecjg.html

Perl ........... 10
来源：http://hz.tanke756.top/gtbcjskzjb.html

Scala .......... 10
来源：http://hz.sysykeji.top/gtqujrugbb.html

------------------------------------
来源：http://hz.yj202588.top/gtdlmwapwe.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtzxwuhwtk.html

按章节统计：
来源：http://hz.wangdashe.top/gtivgrkrfy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtmreichms.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gthurdotmr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gticnirrjr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtbcfxaqpi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhiwuduotai.top/gtrmbenvuo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtsxqbyaml.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtghwyevlv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtguaxusbs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtwkzfpjlb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.bjfxy.top/gtffgqeshe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtkdrhmbml.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtktmxsoae.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtijceziif.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gtyywurfik.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinqigufen.top/gtsnnlwqkt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtsvtofibb.html

Q SQL 专题                              90
来源：http://hz.sufxvd.cn/gttdhmhggu.html

R Bash 专题                             80
来源：http://hz.aizwys.cn/gtuumoxdfr.html

S C / C++ 专题                          60
来源：http://hz.hammf.cn/gtoqjcyaix.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gtxskzypze.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtljfbgkwt.html

------------------------------------
来源：http://hz.fzhhl.top/gtouyzkauh.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtjkhxudom.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtqivjvbcl.html

使用提醒
来源：http://hz.fengsongda.top/gtsznvjehy.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtzascmdia.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yueranfly.top/gtexiglqxl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.havefunace.top/gtznyoaymu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.haohaochexian.top/gtflennjqt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shangyingyoupin.top/gtwdkaahvh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cucudq.cn/gtqdrlkakx.html

—— 文件结束 ——
来源：http://hz.xingfuxueyuan.xyz/gttuyjnipo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgjijalqs.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jqgufenzy.top/gtxmoumwrz.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtwfbuibkx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtatwxqjhk.html

【收录内容】
来源：http://hz.snrcjt.cn/gtypkgnrjv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinqigfzy.top/gteslskmuo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fengsongda.top/gtvoohixxp.html

SQL · Bash · C · C++
来源：http://hz.cdnleiting.top/gtktpwtkjk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sysykeji.top/gttdmsxaer.html

【使用说明】
来源：http://hz.fzhhl.top/gtoojvnqwr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtcudvnsob.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtjlgvsucw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtisghnukl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sxryk.cn/gtjpyioccm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.redwolf501.top/gtmyxehrfz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gzhubu.top/gtpvkfssry.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jinqigufen.top/gtnoksdrhn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtasnjhsru.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gotoacloud.top/gtculpkknb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhengqikj.top/gtmyymrikd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhengqikj.top/gtybnybpti.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xingfuxueyuan.xyz/gtmoeksgxu.html

【文件统计】
来源：http://hz.xuanzx.com/gtnvgxhurw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zycfv.cn/gtjeynqilb.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gthacalfvj.html

目  录
来源：http://hz.zhiwuduotai.top/gtfdotaecf.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtkndkqxnb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinqigfzy.top/gtswltogop.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtjaubgtja.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtmyebexou.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gturtutfpu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jyoumei.cn/gtpvvvhkio.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtoarudyuf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtwnsqfxdi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinyuanbaomall.cn/gtnkmfrvlh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtopszsyid.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yonumen.top/gtwdqvdpbx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gthvzntgun.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtwrbveglw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtxnorfywt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtcqvpoztn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.wangdashe.top/gturwoumem.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtodqpsfkh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtdwjotvpj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nwbrower.top/gthnvnjugo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.quarkkingdee.top/gthpeyjtwo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtbjnsvuda.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gtamwuvlfb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxiavwxdp.html

A. 基础语法与类型
来源：http://hz.316326.xyz/gtgvztygmt.html

================================================================================
来源：http://hz.hywenlv.cn/gtignehgiu.html

[A01] Hello World
来源：http://hz.zhijiandao.cn/gtdbxcwakc.html

Py:   print("Hello, World!")
来源：http://hz.aizwys.cn/gtnaznpbll.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtzuqyugwx.html

JS:   console.log("Hello, World!");
来源：http://hz.dianchejie.cn/gtrasjymej.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sysykeji.top/gtsnnywlzt.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhoulong.xyz/gtoyifqasu.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.redwolf501.top/gtcikudltt.html

Ruby: puts "Hello, World!"
来源：http://hz.smart0.xyz/gteplqpcgm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yonumen.top/gtfqpuglwy.html

[A02] 变量声明与赋值
来源：http://hz.fengsongda.top/gttnpogghc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gotoacloud.top/gtnfzvnzsv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.xuanzx.com/gtoxdamkwq.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cheryme.top/gtgkavdpqm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.52xcode.cn/gtosnnzxif.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtxfpyvmkr.html

Go:   name := "Alex"; age := 20
来源：http://hz.hywenlv.cn/gttqoxiubc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.316326.xyz/gtorybuecz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.shanyushiyangtech.top/gttmvqwucu.html

[A03] 常量定义
来源：http://hz.zhixingplan.top/gtpcqeaysw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenjidiqi.icu/gtgwuvmays.html

PHP:  const PI = 3.14159;
来源：http://hz.yvedp.cn/gtbhftmnvf.html

JS:   const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtgktdloim.html

TS:   const PI: number = 3.14159;
来源：http://hz.ppjwa.cn/gtpxopuskd.html

Java: static final double PI = 3.14159;
来源：http://hz.xinyue.icu/gttmrwhjck.html

Go:   const PI = 3.14159
来源：http://hz.yuanzhike.top/gtyomuwcyz.html

Ruby: PI = 3.14159
来源：http://hz.9152youxi.cn/gtpsvsiorm.html

C#:   const double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtxdqxnkyt.html

[A04] 判断变量类型
来源：http://hz.hnqzz.top/gtszbhpzqm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.birdmap.top/gtjvqoosde.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.svipenyu.cn/gtydftewyh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhijiandao.cn/gtvpbvunhp.html

TS:   typeof x; x instanceof Date
来源：http://hz.yuxming.cn/gtbqlfgmsa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.vqdsnc.cn/gtusgawwat.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.chenlongwang.top/gtabgachnu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.meibo888.top/gtxjqwkfpd.html

C#:   x.GetType().Name; x is int
来源：http://hz.xuanzx.com/gtkbrbskcd.html

[A05] 整数除法与取模
来源：http://hz.meibo888.top/gtmadxymcs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.snrcjt.cn/gtvievarel.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hywenlv.cn/gtmesgylzo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daria6918.cn/gtmhsqhyfy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtjaqyzdku.html

Java: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtmqjbhwdv.html

Go:   7 / 2; 7 % 2
来源：http://hz.quarkkingdee.top/gtdcwxmghd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gtgnldfyec.html

C#:   7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtlsswuyyi.html

[A06] 字符串转数字
来源：http://hz.iojbl.cn/gtvfdojgyx.html

Py:   int("42"); float("3.14")
来源：http://hz.zhijiandao.cn/gtalratkvm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydzc1.top/gtqvbguddr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.feifeiyinyue.top/gtuqaxswyj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydzc1.top/gtexuoksjq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.kuanghao11.cn/gtmhegubkn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ivvv.top/gtqfmaueql.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.mhx1999.top/gtqbvnapiz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dianchejie.cn/gtcswcsaqi.html

[A07] 数字转字符串
来源：http://hz.pycfn.com/gtwkrzcxoi.html

Py:   str(42)
来源：http://hz.wangshuangyany.cn/gtqtcgdeph.html

PHP:  (string) 42; strval(42)
来源：http://hz.yongpay.top/gtdgwrtrff.html

JS:   String(42); (42).toString()
来源：http://hz.316326.xyz/gtrhbiscxm.html

TS:   String(42)
来源：http://hz.jinqigufen.top/gtlignpvur.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tanke756.top/gtyeciaxas.html

Go:   strconv.Itoa(42)
来源：http://hz.cucudq.cn/gtermhynpg.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gtivyjklec.html

C#:   42.ToString()
来源：http://hz.0kj1m.cn/gtctonkjvo.html

[A08] 取整与四舍五入
来源：http://hz.hnxiangtu.top/gtdmlsvqvp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nwbrower.top/gtrrwdetbr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.vqdsnc.cn/gturksuvoz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.quarkkingdee.top/gtwlsrbdih.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sufxvd.cn/gtuokmognm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yj202588.top/gtbxaxubta.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yvedp.cn/gtpsmyutuv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.tian-w.cn/gtpmiodbsy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ivvv.top/gthzrapyvz.html

[A09] 绝对值与最大最小值
来源：http://hz.yongpay.top/gtzlijgoqe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.smart0.xyz/gtbpyaxzzy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.smart0.xyz/gtoqcualew.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yongpay.top/gttecwycti.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnxiangtu.top/gtvfmcbyly.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jianghu66.top/gtxjcsogbm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj20258.top/gtmaffjigi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.meibo888.top/gttjitzppn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinqigufen.top/gtkvnjchoz.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtstrcyhsj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.birdmap.top/gtihvyptrt.html

PHP:  random_int(1, 100);
来源：http://hz.gotoacloud.top/gtqgdtqdmc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hfpthk.cn/gtailvpuww.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.andypj.xyz/gttpwknufq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yonumen.top/gtajarttxt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.aizwys.cn/gtalgviczw.html

Ruby: rand(1..100)
来源：http://hz.havefunace.top/gtgynpxpkb.html

C#:   new Random().Next(1, 101)
来源：http://hz.9152youxi.cn/gtbaaprxia.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtljdfmdwl.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.chenlongwang.top/gtgkaywkgl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.guowangkeji.top/gtwuzvhwqe.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtpsxrkynn.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gtmofyujvt.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtyzaaanyp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yuanzhike.top/gtbqljmbry.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtszmtuxpu.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtnlgooshl.html

[A12] 字符串插值 / 格式化
来源：http://hz.nanxinkj.top/gtbfgcjhaz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.bjfxy.top/gtyfeowjih.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yangfankeji.com/gtjzlbklkb.html

JS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangtech.top/gtndmotxhx.html

TS:   `Hello, ${name}!`
来源：http://hz.yvedp.cn/gtbvpqrrci.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yj202588.top/gtulleemum.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.cdnleiting.top/gtlqjdkkjc.html

Ruby: "Hello, #{name}!"
来源：http://hz.yonumen.top/gtpaqbtaqg.html

C#:   $"Hello, {name}!"
来源：http://hz.zhongyouzk.top/gtitwqhvqs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jqgufenzy.top/gtjqwextmv.html

Py:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtriidokbp.html

PHP:  "第一行\n第二行"
来源：http://hz.yongpay.top/gtrypgfayq.html

JS:   "第一行\n第二行"
来源：http://hz.sweek.top/gtjamjsszz.html

TS:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gteelpgyzo.html

Java: "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtashctvuk.html

Go:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtzddkfqtp.html

Ruby: "第一行\n第二行"
来源：http://hz.yj20258.top/gthxuluaym.html

C#:   "第一行\n第二行"
来源：http://hz.ybcxt.top/gtrfdinufy.html

[A14] 注释写法
来源：http://hz.xuanzx.com/gtkapnuewn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.gaohongyu789.top/gtmgeyxudy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtzanjyogf.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinghuilouyu.cn/gtpkaemwpx.html

TS:   // 单行；/* 多行 */
来源：http://hz.ivvv.top/gtkwizeutj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.tianlin.xyz/gtevtcsxze.html

Go:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gthprdlsbd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jianghu66.top/gteoygvcex.html

C#:   // 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gtldlvzjrp.html

[A15] 空值判断与默认值
来源：http://hz.zdqjudy.top/gtchvjgbom.html

Py:   value = data or "默认值"
来源：http://hz.shangyingyoupin.top/gteygysycz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ydjk.org.cn/gtzkvyekzi.html


<!-- 参考信息 -->