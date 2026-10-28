代发 wailian999

[U87] JS：解构默认值
来源：http://hz.zhixingplan.top/gtqpsqsiem.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zdqjudy.top/gtbbcnokck.html

[U88] JS：对象展开合并
来源：http://hz.yvedp.cn/gtiomozslv.html

{ ...a, ...b }
来源：http://hz.yj202588.top/gtoyfwcycv.html

[U89] JS：数组去重
来源：http://hz.xuanzx.com/gtskwjrpsz.html

[...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtqmrfdgwr.html

[U90] JS：数字数组排序
来源：http://hz.0kj1m.cn/gtdjloulif.html

[...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtnpidzyfv.html

[U91] JS：对象键值遍历
来源：http://hz.zhaomingkeji.xyz/gtymruezar.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ehwqpu.com/gtebjbatpp.html

[U92] JS：深拷贝
来源：http://hz.bjfxy.top/gtplmgtptq.html

structuredClone(obj)
来源：http://hz.ydzc1.top/gtomredajm.html

[U93] JS：模板字符串
来源：http://hz.tanke756.top/gtvqsrmtpw.html

`共 ${n} 条`
来源：http://hz.jqgufenzy.top/gtjzttgnlj.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtjpkycqgs.html

const double = x => x * 2;
来源：http://hz.yanxiufei.cn/gtyeerdmkd.html

[U95] JS：Promise 包装
来源：http://hz.9152youxi.cn/gtuiofioho.html

new Promise((resolve, reject) => {})
来源：http://hz.cqqwz.cn/gtutejkvfe.html

[U96] JS：async/await 与异常
来源：http://hz.guannengcc.top/gtnwzqluos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtwclwasct.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtjtgebliy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtidwewrag.html

[U98] JS：fetch 带 JSON
来源：http://hz.mhx1999.top/gtrqjevuma.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtljnumgfx.html

[U99] JS：事件监听
来源：http://hz.xinyue.icu/gtrfraeknp.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtoosbmprq.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtxkbmprdn.html

document.querySelector(".item")
来源：http://hz.gogol.net.cn/gtzkrqmefv.html

[U101] JS：classList 操作
来源：http://hz.xuetiantiany.cn/gtcphvnklq.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtlszgnhce.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gtvwzhanft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xingfuxueyuan.xyz/gtnoycirhd.html

[U103] JS：定时器
来源：http://hz.pengpengdd.cyou/gtxppwtlhf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jqgfzy.top/gtqacgvjzy.html

[U104] JS：防抖
来源：http://hz.c1oappe.top/gtgxjtzvxt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtnhvzpcil.html

[U105] JS：节流
来源：http://hz.vqdsnc.cn/gtpygfmfnp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgfzy.top/gtusfbfqzl.html

[U106] JS：日期格式化
来源：http://hz.yj202588.top/gtgkywablu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.feifeiyinyue.top/gtedzsbmdb.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gtlypusmzb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.c1oappe.top/gtymabzcva.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gtlhjselrj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gthlrtttci.html

[U109] JS：数组分组
来源：http://hz.jqgfzy.top/gtcofcayjr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtdyrqdlkl.html

[U110] JS：数组分块
来源：http://hz.xuetiantiany.cn/gtghnijyrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jianghu66.top/gtubfgyqhv.html

[U111] JS：对象转 Map
来源：http://hz.cashguo.top/gtwsvzrpkl.html

new Map(Object.entries(obj))
来源：http://hz.shzxlz.cn/gtcisbqyfh.html

[U112] JS：字符串补位
来源：http://hz.guannengcc.top/gttxugmiba.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtwktnxbkr.html

[U113] JS：正则替换全部
来源：http://hz.hysaishi.cn/gtxsrvfnmf.html

s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtfvxllydd.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gttnvhwtpe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtigfphkjn.html

[U115] JS：生成 UUID
来源：http://hz.quarkkingdee.top/gtssqyxohk.html

crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtmlgscpsd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhoulong.xyz/gtreohczsj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gtrhtbgxwh.html

[U117] JS：单元测试
来源：http://hz.kuanghao11.cn/gtmgtmfoax.html

npm i -D vitest;  npx vitest
来源：http://hz.gaohongyu789.top/gtfjmqrnvt.html

[U118] JS：开发服务器
来源：http://hz.ydjk.org.cn/gtvzzewxds.html

npm i -D vite;  npx vite
来源：http://hz.hongshengwenyu.top/gtwzrbbqgo.html

[U119] JS：生产构建
来源：http://hz.zhengqikj.top/gtrqcprlzf.html

npx vite build
来源：http://hz.cqqwz.cn/gtzdekpsxk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtrikazeha.html

import.meta.env.VITE_API_URL
来源：http://hz.ydzc1.top/gtbeevgoim.html

================================================================================
来源：http://hz.shzxlz.cn/gtdfksrgyw.html

统计汇总
来源：http://hz.fzhhl.top/gtpqxybaqc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtabbhnmzd.html

按语言统计（条）：
来源：http://hz.ivvv.top/gtrkiuewdn.html

Python ......... 252
来源：http://hz.svipenyu.cn/gtqhahhwny.html

PHP ............ 252
来源：http://hz.yangfankeji.com/gtceidzfvm.html

JavaScript ..... 252
来源：http://hz.svipenyu.cn/gthbecgqrr.html

TypeScript ..... 212
来源：http://hz.jinqigufen.top/gtnahhaaov.html

Java ........... 212
来源：http://hz.9152youxi.cn/gttzmwogay.html

Go ............. 212
来源：http://hz.chenjidiqi.icu/gteudiiflb.html

Ruby ........... 212
来源：http://hz.yuanzhike.top/gtfpciyunu.html

C# ............. 212
来源：http://hz.jinghuilouyu.cn/gtqtfychwk.html

C .............. 30
来源：http://hz.jinqigufen.top/gtrfkyfght.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtwbrfadnj.html

SQL ............ 90
来源：http://hz.sweek.top/gtlancmzbk.html

Bash ........... 80
来源：http://hz.xuetiantiany.cn/gtfjnhndju.html

Kotlin ......... 15
来源：http://hz.gogol.net.cn/gtygojawvv.html

Swift .......... 15
来源：http://hz.chenzaomai.com/gtwqunhrpu.html

Lua ............ 10
来源：http://hz.yangfankeji.com/gtpdxgrvcy.html

Perl ........... 10
来源：http://hz.cqqwz.cn/gtbhiqqway.html

Scala .......... 10
来源：http://hz.ydzc1.top/gtpntbbbrf.html

------------------------------------
来源：http://hz.zhiwuduotai.top/gtpcexnpun.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gtofppffwf.html

按章节统计：
来源：http://hz.ehwqpu.com/gtfkfaifnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtjxdxtoaj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtxzywhsei.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtaweqmxkx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtbtcvyxrj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yangfankeji.com/gttubsanfp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtpycsbxfq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtqtotocdp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtujrivgfc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtmumddjjk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ivvv.top/gtwpntcvtw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gthmvpxtzv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtajnomaqg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtjzdhfpph.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258.top/gtcurdmkqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gzhubu.top/gtzotimnre.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtmhnscdgd.html

Q SQL 专题                              90
来源：http://hz.gogol.net.cn/gtpzawcgda.html

R Bash 专题                             80
来源：http://hz.xinyue.icu/gtftvjshbw.html

S C / C++ 专题                          60
来源：http://hz.jyoumei.cn/gtdfsmiiow.html

T 其他语言补充                          60
来源：http://hz.dianchejie.cn/gtrtuhkmug.html

U 高频实用片段                         120
来源：http://hz.yanxiufei.cn/gtmxiqmpiq.html

------------------------------------
来源：http://hz.jqgfzy.top/gtedjahrof.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtbpbtbtga.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtaxwnhbcr.html

使用提醒
来源：http://hz.yuanzhike.top/gtnghrrhkt.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gttznbrjlr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tian-w.cn/gtvqklaqkk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hysaishi.cn/gtnixeuqlp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jlsjyb.cn/gtsldljndl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtzmlwfpfu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.feifeiyinyue.top/gtohckqudo.html

—— 文件结束 ——
来源：http://hz.zhaomingkeji.xyz/gtfinvoweh.html

================================================================================
来源：http://hz.wangdashe.top/gtjarhcooh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.shzxlz.cn/gtgqrcxrya.html

Common Programming Examples Cheat Book
来源：http://hz.cashguo.top/gtvleoxxve.html

================================================================================
来源：http://hz.9152youxi.cn/gtpifkoavt.html

【收录内容】
来源：http://hz.jinqigufen.top/gtcsjnpgrl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhengqikj.top/gtkpngfrqd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.bjfxy.top/gtwleivwxh.html

SQL · Bash · C · C++
来源：http://hz.shanyushiyangkeji.top/gtrkgyires.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sufxvd.cn/gtyqkohfro.html

【使用说明】
来源：http://hz.jqgufenzy.top/gtcxbofhhp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangshuangyany.cn/gtydfgrtbc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhiwuduotai.top/gthdyfkkin.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtymmwpxas.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jianghu66.top/gtgyagctyw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.quarkkingdee.top/gtmsfkwupa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zycfv.cn/gtilrwkbyi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ppjwa.cn/gterqaxeme.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xziqi.cn/gtjplsstfb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenlongwang.top/gtqpevzeck.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.smart0.xyz/gtrmxdrgah.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.316326.xyz/gtttdjsbgv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sweek.top/gtglgmzrcy.html

【文件统计】
来源：http://hz.guowangkeji.top/gtzoexllsq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cqqwz.cn/gtrwgrzapz.html

--------------------------------------------------------------------------------
来源：http://hz.ehwqpu.com/gthtanlzyr.html

目  录
来源：http://hz.316326.xyz/gtpelgfrgp.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtycdenknw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenlongwang.top/gtormsegvn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtkmimpbon.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtoycazaxb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtpscasruz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yuanzhike.top/gtogrrhfzy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cqqwz.cn/gtkgaxzron.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtvxfswxqf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sxryk.cn/gtkbznrrrl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtazaeedmy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtrlflgaiy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtoidnrdrx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtmsypitlq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtbwkiruus.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtreufwfoc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shuidangran.top/gtrtmdmwih.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtcksklioc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.havefunace.top/gtgiijylvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhixingplan.top/gtvrvxgoul.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.daxiang520.top/gtikmmhpvj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtddqlohsv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtxrpitbio.html

================================================================================
来源：http://hz.zhengqikj.top/gtzsawrmdi.html

A. 基础语法与类型
来源：http://hz.yonumen.top/gtsxcqpscl.html

================================================================================
来源：http://hz.zdqjudy.top/gtvmthbdlo.html

[A01] Hello World
来源：http://hz.xingfuxueyuan.xyz/gtlwuyhybo.html

Py:   print("Hello, World!")
来源：http://hz.yj202588.top/gtrpvrsows.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtkqpdbdcl.html

JS:   console.log("Hello, World!");
来源：http://hz.yj20258888.top/gtordukhpi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yvedp.cn/gtoavukhio.html

Java: System.out.println("Hello, World!");
来源：http://hz.jyoumei.cn/gtymrfbkkj.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj202588.top/gthfbqdapo.html

Ruby: puts "Hello, World!"
来源：http://hz.cqqwz.cn/gtyugxuhxj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinghuilouyu.cn/gtegzncqaw.html

[A02] 变量声明与赋值
来源：http://hz.jianghu66.top/gtirfdtrqp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gtdhachmse.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hfpthk.cn/gtvdgpmqek.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.quarkkingdee.top/gtvdemmxhh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shuidangran.top/gtzllstnxh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daxiang520.top/gtxdcwrrwq.html

Go:   name := "Alex"; age := 20
来源：http://hz.feifeiyinyue.top/gtofhgogag.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cashguo.top/gtstuofzvq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.wangdashe.top/gtzgmkzlve.html

[A03] 常量定义
来源：http://hz.jinqigufen.top/gtehbkwywi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.iojbl.cn/gtmffecfmb.html

PHP:  const PI = 3.14159;
来源：http://hz.ppjwa.cn/gtlxbxgchu.html

JS:   const PI = 3.14159;
来源：http://hz.c1oappe.top/gtoqgtkzyd.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtznykkzqb.html

Java: static final double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtcnaymgxj.html

Go:   const PI = 3.14159
来源：http://hz.guannengcc.top/gtmvljaujq.html

Ruby: PI = 3.14159
来源：http://hz.xinyue.icu/gtsmhxipxq.html

C#:   const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtxqijafrk.html

[A04] 判断变量类型
来源：http://hz.jiagoushi.top/gteqaznnis.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.9152youxi.cn/gtindbcsia.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guowangkeji.top/gtekbevdwd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sufxvd.cn/gtbxjogrro.html

TS:   typeof x; x instanceof Date
来源：http://hz.vqdsnc.cn/gtznmvlnfg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shanyushiyangtech.top/gttbzmyncr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hammf.cn/gtpeeguygi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhixingplan.top/gtguakpyuk.html

C#:   x.GetType().Name; x is int
来源：http://hz.guowangkeji.top/gtiebtzznt.html

[A05] 整数除法与取模
来源：http://hz.jinqigfzy.top/gtcjyfpuar.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.9152youxi.cn/gtnfibfxkb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.dianchejie.cn/gtnqmxdicb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtnxlpdboi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yanxiufei.cn/gtaemgkfzm.html

Java: 7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtfpwzcnhu.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtptegnjey.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtfqwxerbj.html

C#:   7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gttrbijpmj.html

[A06] 字符串转数字
来源：http://hz.jinghuilouyu.cn/gtrhiwiwlq.html

Py:   int("42"); float("3.14")
来源：http://hz.hfpthk.cn/gtyjaqgcus.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.tianlin.xyz/gtiioogzwo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenjidiqi.icu/gtmxqsboeq.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.0kj1m.cn/gtzeoxhrlu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.52xcode.cn/gtamzdiphm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.dashuyun.cn/gtcfzmjrjw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.pycfn.com/gtqwgdtdwe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhoulong.xyz/gtlsvwtcko.html

[A07] 数字转字符串
来源：http://hz.shanyushiyangkeji.top/gtrctfsrub.html

Py:   str(42)
来源：http://hz.smart0.xyz/gtyvafqehr.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhengqikj.top/gtrtidywcz.html

JS:   String(42); (42).toString()
来源：http://hz.hnqzz.top/gtapcrcafz.html

TS:   String(42)
来源：http://hz.jqgfzy.top/gtjnxbwpii.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.iojbl.cn/gthxunmcvh.html

Go:   strconv.Itoa(42)
来源：http://hz.gzhubu.top/gtniwufemk.html

Ruby: 42.to_s
来源：http://hz.jinqigufen.top/gtvwsyktth.html

C#:   42.ToString()
来源：http://hz.wangdashe.top/gtzguaxfnn.html

[A08] 取整与四舍五入
来源：http://hz.xuetiantiany.cn/gtwxjbwwbf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shangyingyoupin.top/gtinmidnza.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.haohaochexian.top/gthbidtwej.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhengqikj.top/gtuqavxreu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sufxvd.cn/gtyqfsgvja.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gtquyhdrnd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.bjfxy.top/gtzmiskfdm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cdnleiting.top/gtssfphlgy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hnqzz.top/gtlddsupgz.html

[A09] 绝对值与最大最小值
来源：http://hz.xziqi.cn/gtwcgybvki.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuxming.cn/gtosceylmq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtziidxhji.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhoulong.xyz/gtdvntelwt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.wangshuangyany.cn/gtdkvvlcqr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xuetiantiany.cn/gtpsyqnhck.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.bjfxy.top/gtliljbwdd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.mhx1999.top/gtiuotruld.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yonumen.top/gtydtxakwf.html

[A10] 生成随机数
来源：http://hz.shuidangran.top/gtitfrmswt.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yj20258888.top/gtbpvupgvf.html

PHP:  random_int(1, 100);
来源：http://hz.xinyue.icu/gtqqhdedsq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xinyue.icu/gtvcmdwpay.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shanyushiyangtech.top/gtlmzdbzua.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yvedp.cn/gtqjdiottj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shuidangran.top/gtqdihyqdh.html

Ruby: rand(1..100)
来源：http://hz.xuanzx.com/gtasihzjzw.html

C#:   new Random().Next(1, 101)
来源：http://hz.chenlongwang.top/gtkgmixrlo.html

[A11] 条件表达式（三元）
来源：http://hz.jqgufenzy.top/gtknaftmuo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhoulong.xyz/gtrysdbsiu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.redwolf501.top/gtgriyhzua.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.xziqi.cn/gtoywgzqpo.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtixmfnshc.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhoulong.xyz/gtvxiahnwp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xuetiantiany.cn/gtivlrthrv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xuetiantiany.cn/gtkkxnscfs.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtmpahwjry.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhijiandao.cn/gtofktgqef.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yuanzhike.top/gtwgevykxg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yj202588.top/gtthalgnye.html

JS:   `Hello, ${name}!`
来源：http://hz.zhiwuduotai.top/gtghofvmxs.html

TS:   `Hello, ${name}!`
来源：http://hz.shangyingyoupin.top/gthsbflbnn.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hnxiangtu.top/gtocysxsvw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jinyuanbaomall.cn/gtfwbqkpjm.html

Ruby: "Hello, #{name}!"
来源：http://hz.hnqzz.top/gtllglyita.html

C#:   $"Hello, {name}!"
来源：http://hz.cheryme.top/gtcmvuivtw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.kuanghao11.cn/gtqsmnpwre.html

Py:   "第一行\n第二行"
来源：http://hz.zhiwuduotai.top/gtxvnpsvmz.html

PHP:  "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtsucvrqcb.html

JS:   "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtoalhspqg.html

TS:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtrlalcjzr.html

Java: "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtiymzcgcz.html

Go:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gttuddseow.html

Ruby: "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtrfoumely.html

C#:   "第一行\n第二行"
来源：http://hz.fzhhl.top/gtkvoivqjt.html

[A14] 注释写法
来源：http://hz.guowangkeji.top/gtpcxhokol.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.pengpengdd.cyou/gtxychrreb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtfipventp.html

JS:   // 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtakusgaif.html

TS:   // 单行；/* 多行 */
来源：http://hz.yvedp.cn/gteolzhtab.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinghuilouyu.cn/gtbazvpohy.html

Go:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtastimwka.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hammf.cn/gtmtyerjix.html


<!-- 参考信息 -->