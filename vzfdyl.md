代发 wailian999

[U85] JS：可选链
来源：http://hz.sufxvd.cn/gtepwydmku.html

a?.b?.c
来源：http://hz.316326.xyz/gtjcmylzdt.html

[U86] JS：空值合并
来源：http://hz.xinyue.icu/gtillazmxw.html

a ?? b
来源：http://hz.shangyingyoupin.top/gtwejrhohn.html

[U87] JS：解构默认值
来源：http://hz.gaohongyu789.top/gtfazvwalz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnxiangtu.top/gtyestqxxg.html

[U88] JS：对象展开合并
来源：http://hz.ydjk.org.cn/gtnjunnrad.html

{ ...a, ...b }
来源：http://hz.shanyushiyangtech.top/gtlglgayyy.html

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtbcdivcuw.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtmwlwetvr.html

[U90] JS：数字数组排序
来源：http://hz.yvedp.cn/gtubkniiig.html

[...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtwlfzgbxt.html

[U91] JS：对象键值遍历
来源：http://hz.yangfankeji.com/gtygxtjmma.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenzaomai.com/gtdvkiqlbj.html

[U92] JS：深拷贝
来源：http://hz.pycfn.com/gtxvxthejq.html

structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtliokunvl.html

[U93] JS：模板字符串
来源：http://hz.snrcjt.cn/gtzduomcik.html

`共 ${n} 条`
来源：http://hz.xziqi.cn/gtgpouphvu.html

[U94] JS：箭头函数
来源：http://hz.yj202588.top/gtvhnudokw.html

const double = x => x * 2;
来源：http://hz.ywan-chungtsiang.top/gtqxmwficp.html

[U95] JS：Promise 包装
来源：http://hz.jinqigfzy.top/gtenuznswy.html

new Promise((resolve, reject) => {})
来源：http://hz.jqgufenzy.top/gtejgemias.html

[U96] JS：async/await 与异常
来源：http://hz.c1oappe.top/gtuoxxbpig.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtmouxamlz.html

[U97] JS：并发请求
来源：http://hz.zycfv.cn/gtxhmzqydk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtcgtyjamh.html

[U98] JS：fetch 带 JSON
来源：http://hz.xylfe.cn/gtyagctgsp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shangyingyoupin.top/gtwqxcsxub.html

[U99] JS：事件监听
来源：http://hz.chenlongwang.top/gtxntndgmg.html

el.addEventListener("click", e => {})
来源：http://hz.dianchejie.cn/gtynhzkgzq.html

[U100] JS：DOM 查询
来源：http://hz.redwolf501.top/gtwpwkgjqt.html

document.querySelector(".item")
来源：http://hz.chenzaomai.com/gtqmcprgza.html

[U101] JS：classList 操作
来源：http://hz.ehwqpu.com/gtdggdyxlt.html

el.classList.toggle("active")
来源：http://hz.andypj.xyz/gtedkkeyvp.html

[U102] JS：本地存储
来源：http://hz.jqgufenzy.top/gtshszbmbf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnxiangtu.top/gtmfyvbjua.html

[U103] JS：定时器
来源：http://hz.ydzc1.top/gtdrwqatwy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sufxvd.cn/gtldyhlseu.html

[U104] JS：防抖
来源：http://hz.shzxlz.cn/gttnrfqbjr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtjdcrttqo.html

[U105] JS：节流
来源：http://hz.dianchejie.cn/gtmgmsklsu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pycfn.com/gtmtcleypk.html

[U106] JS：日期格式化
来源：http://hz.jqgufenzy.top/gtmirubivu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.andypj.xyz/gtyenpuyqu.html

[U107] JS：数字千分位
来源：http://hz.zycfv.cn/gtvetuvofd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xuetiantiany.cn/gtdrfiitkh.html

[U108] JS：随机整数
来源：http://hz.sufxvd.cn/gtbghqmkhr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.c1oappe.top/gttcoteonh.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtsbvhlaap.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtymkyuptm.html

[U110] JS：数组分块
来源：http://hz.fengsongda.top/gtveyyaehl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gtctyazdlg.html

[U111] JS：对象转 Map
来源：http://hz.tian-w.cn/gtumodpybm.html

new Map(Object.entries(obj))
来源：http://hz.quarkkingdee.top/gtwxeudsfo.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtskrnpait.html

"7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtorfelafz.html

[U113] JS：正则替换全部
来源：http://hz.zhijiandao.cn/gtplckykvb.html

s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtydxxyqdg.html

[U114] JS：JSON 深比较
来源：http://hz.jyoumei.cn/gtjbpkifqs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtpxemxvxw.html

[U115] JS：生成 UUID
来源：http://hz.guowangkeji.top/gtlxwziwic.html

crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtnamifgzx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtwhyavvdv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ybcxt.top/gtppwnjiee.html

[U117] JS：单元测试
来源：http://hz.jiagoushi.top/gtklebhxzg.html

npm i -D vitest;  npx vitest
来源：http://hz.dianchejie.cn/gtvrhfbzuf.html

[U118] JS：开发服务器
来源：http://hz.hnqzz.top/gtgtcspzmg.html

npm i -D vite;  npx vite
来源：http://hz.aibaodan.cn/gtnrhlblpq.html

[U119] JS：生产构建
来源：http://hz.meibo888.top/gtpltjjhpy.html

npx vite build
来源：http://hz.gaohongyu789.top/gtsmnbwwfx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.snrcjt.cn/gtbuqajkvl.html

import.meta.env.VITE_API_URL
来源：http://hz.hnqzz.top/gtbbwzoctj.html

================================================================================
来源：http://hz.yj202588.top/gtjgwcwgsb.html

统计汇总
来源：http://hz.0kj1m.cn/gtekiwsdne.html

================================================================================
来源：http://hz.xziqi.cn/gtjklokgll.html

按语言统计（条）：
来源：http://hz.sweek.top/gtlomhzsrs.html

Python ......... 252
来源：http://hz.yuxming.cn/gtrcosrhxr.html

PHP ............ 252
来源：http://hz.yangfankeji.com/gtbivdzxjq.html

JavaScript ..... 252
来源：http://hz.ybcxt.top/gtwjhuyusr.html

TypeScript ..... 212
来源：http://hz.iojbl.cn/gtyxftywwo.html

Java ........... 212
来源：http://hz.bjfxy.top/gtmepkdgpv.html

Go ............. 212
来源：http://hz.zhixingplan.top/gtrxnpzhdc.html

Ruby ........... 212
来源：http://hz.shuidangran.top/gtdudjtzhx.html

C# ............. 212
来源：http://hz.fzhhl.top/gtnujucgma.html

C .............. 30
来源：http://hz.yj202588.top/gtfpemdtng.html

C++ ............ 30
来源：http://hz.iojbl.cn/gtvhcbvnsi.html

SQL ............ 90
来源：http://hz.jinghuilouyu.cn/gtcpqdoujb.html

Bash ........... 80
来源：http://hz.shangyingyoupin.top/gtgkfjbbvt.html

Kotlin ......... 15
来源：http://hz.hywenlv.cn/gtbgghmszc.html

Swift .......... 15
来源：http://hz.yanxiufei.cn/gtkbpxduad.html

Lua ............ 10
来源：http://hz.c1oappe.top/gtyrcfipps.html

Perl ........... 10
来源：http://hz.chenjidiqi.icu/gtztqkmjdl.html

Scala .......... 10
来源：http://hz.xingfuxueyuan.xyz/gtvhttchlp.html

------------------------------------
来源：http://hz.dianchejie.cn/gtvxqmduoq.html

合计 ........... 2106 条
来源：http://hz.hammf.cn/gtrendlgnm.html

按章节统计：
来源：http://hz.guannengcc.top/gtxuntdkdu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtyhusbfay.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtewnilafa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtbqkmblwb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtmdegaxuc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhiwuduotai.top/gtpdcghchu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtbepztgeo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gthbsgdquk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gthsjftnxn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtbazldzqo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtknyvjnof.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtatsumjub.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtvneaiqig.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtrokhepwk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xinyue.icu/gtfilzgdqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.mhx1999.top/gtgdrpuacf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtqlawgxkd.html

Q SQL 专题                              90
来源：http://hz.hnqzz.top/gtrriimuvt.html

R Bash 专题                             80
来源：http://hz.mhx1999.top/gtzeuewqxy.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtxowwiask.html

T 其他语言补充                          60
来源：http://hz.yanxiufei.cn/gtscyphwhn.html

U 高频实用片段                         120
来源：http://hz.daria6918.cn/gtfnprdkfn.html

------------------------------------
来源：http://hz.jlsjyb.cn/gtisdihlkg.html

合计                                  2106 条
来源：http://hz.jinqigfzy.top/gtshjnkuje.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtkihzdxjh.html

使用提醒
来源：http://hz.cheryme.top/gtiuxiiuky.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtydlpptbk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cheryme.top/gtpktymwtf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.snrcjt.cn/gtpcumkvid.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtwzoawaif.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sysykeji.top/gtfrumiope.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guowangkeji.top/gtdeqzeagk.html

—— 文件结束 ——
来源：http://hz.dashuyun.cn/gtqvzuhprc.html

================================================================================
来源：http://hz.sweek.top/gtnrmhvtok.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hongshengwenyu.top/gtepdxlrbj.html

Common Programming Examples Cheat Book
来源：http://hz.shanyushiyangkeji.top/gtmroijmih.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gteyrlhgby.html

【收录内容】
来源：http://hz.hammf.cn/gtaoqjxzap.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ydzc1.top/gtlqgsifla.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.vqdsnc.cn/gtkblqgysr.html

SQL · Bash · C · C++
来源：http://hz.xuanzx.com/gtlsgpqpzp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhoulong.xyz/gtwfmehcvw.html

【使用说明】
来源：http://hz.ivvv.top/gtmnmgygry.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhiwuduotai.top/gtmgaijtkj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yvedp.cn/gtwxemgtfk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xylfe.cn/gtrbmxylwj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zdqjudy.top/gthcpcwwgj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.fzhhl.top/gtqaewevzi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuanzhike.top/gtjdavogfa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gotoacloud.top/gtrlowixuy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yanxiufei.cn/gtrnyfwott.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.gzhubu.top/gtbkowjipp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ydzc1.top/gttjfmwjwy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhaomingkeji.xyz/gtrxrpsptc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cucudq.cn/gtdwcmveib.html

【文件统计】
来源：http://hz.yuanzhike.top/gtsmzyknpu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xylfe.cn/gthzzwweyx.html

--------------------------------------------------------------------------------
来源：http://hz.meibo888.top/gtlormuefo.html

目  录
来源：http://hz.fengsongda.top/gtpqkqfuun.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtlvtapkgj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.meibo888.top/gtkebuqtep.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtjmeeervg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydzc1.top/gttysdgdli.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtddohcmsk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aizwys.cn/gtzmsqujck.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.feifeiyinyue.top/gthlalpdrz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtxbaskxil.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gttxsnewgc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtgnvuhyed.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gtknkzhzbm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtscmqfmgd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtsiglpkvs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.redwolf501.top/gtaqwagbtu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gthmaufill.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj202588.top/gtmzcfhnrp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtuntohqif.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258888.top/gtzmltrsjh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yongpay.top/gtbsgbjiwc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gotoacloud.top/gthhpelwac.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtfmlhxvyv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtnxljhyug.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxefhcndm.html

A. 基础语法与类型
来源：http://hz.guowangkeji.top/gtzexgankb.html

================================================================================
来源：http://hz.ehwqpu.com/gtwsghoylo.html

[A01] Hello World
来源：http://hz.gzhubu.top/gtfkhlahpc.html

Py:   print("Hello, World!")
来源：http://hz.chenlongwang.top/gtfzvypeip.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtxpvmarhj.html

JS:   console.log("Hello, World!");
来源：http://hz.ydzc1.top/gtghpcqalu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jlsjyb.cn/gtchlqtxms.html

Java: System.out.println("Hello, World!");
来源：http://hz.aibaodan.cn/gtnhhsicmq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenzaomai.com/gtpqvjctiq.html

Ruby: puts "Hello, World!"
来源：http://hz.chenjidiqi.icu/gtvmlulxba.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.vqdsnc.cn/gtktifyytc.html

[A02] 变量声明与赋值
来源：http://hz.hywenlv.cn/gtutoiisph.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yangfankeji.com/gtqekejgol.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.havefunace.top/gtboverags.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj20258888.top/gtutflvlnk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.vqdsnc.cn/gtzqwzvxsi.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gtwhvfwxrt.html

Go:   name := "Alex"; age := 20
来源：http://hz.iojbl.cn/gttrqkrhlq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.dianchejie.cn/gtbpdrlorz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtlgcxfmei.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtghwjsary.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yongpay.top/gtfcgavqlx.html

PHP:  const PI = 3.14159;
来源：http://hz.aizwys.cn/gtwlxkfqxw.html

JS:   const PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtruetughm.html

TS:   const PI: number = 3.14159;
来源：http://hz.ydjk.org.cn/gtpwnqdhty.html

Java: static final double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtkxckjsqb.html

Go:   const PI = 3.14159
来源：http://hz.shuidangran.top/gtdbmjntjy.html

Ruby: PI = 3.14159
来源：http://hz.ybcxt.top/gtcudpufiu.html

C#:   const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtzortblud.html

[A04] 判断变量类型
来源：http://hz.jyoumei.cn/gtzhzaghkn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.0kj1m.cn/gtolwmzyws.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daxiang520.top/gtylgilhnd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnqzz.top/gtzzmnzkgo.html

TS:   typeof x; x instanceof Date
来源：http://hz.vqdsnc.cn/gtbenrbemj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.fzhhl.top/gtgdfptpdl.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gtswfdzolo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxuanxn.top/gtfoohgggi.html

C#:   x.GetType().Name; x is int
来源：http://hz.tanke756.top/gtuxciumzx.html

[A05] 整数除法与取模
来源：http://hz.jlsjyb.cn/gtbzrjzwcw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.birdmap.top/gtfthtufbw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aizwys.cn/gtdpuabnyg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.haohaochexian.top/gtcbbrwxab.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fengsongda.top/gtargodxfg.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gticrinkxc.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gttlklflly.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtjksfyxzs.html

C#:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtqspapclb.html

[A06] 字符串转数字
来源：http://hz.sysykeji.top/gtptnwmeqy.html

Py:   int("42"); float("3.14")
来源：http://hz.birdmap.top/gtcygmfrjh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.svipenyu.cn/gtezedppdw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cucudq.cn/gtevcrpcdm.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.fengsongda.top/gtndmzgrcv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinyuanbaomall.cn/gtjuvigwja.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtyjiurzvi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.dashuyun.cn/gtjgfjvupg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.chenjidiqi.icu/gtqmbjdeie.html

[A07] 数字转字符串
来源：http://hz.mhx1999.top/gtrldnldbg.html

Py:   str(42)
来源：http://hz.zycfv.cn/gtxqzsbdnf.html

PHP:  (string) 42; strval(42)
来源：http://hz.chenzaomai.com/gtrvbzbdwe.html

JS:   String(42); (42).toString()
来源：http://hz.vqdsnc.cn/gtslyelves.html

TS:   String(42)
来源：http://hz.ppjwa.cn/gtwvrmkhgk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gotoacloud.top/gtwthfbuow.html

Go:   strconv.Itoa(42)
来源：http://hz.zhaomingkeji.xyz/gtvgptdrhc.html

Ruby: 42.to_s
来源：http://hz.yj202588.top/gtazlaodtu.html

C#:   42.ToString()
来源：http://hz.ydzc1.top/gtwjjgilwe.html

[A08] 取整与四舍五入
来源：http://hz.fzhhl.top/gtdzzksjtv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.c1oappe.top/gtmwxhidnp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.vqdsnc.cn/gtylhczrdi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtkrpjtfvo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.snrcjt.cn/gtzmdfxhid.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.tanke756.top/gtdzymzvqu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.smart0.xyz/gtjclztmkv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenzaomai.com/gtxcqragwk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hammf.cn/gtaqymeowl.html

[A09] 绝对值与最大最小值
来源：http://hz.ivvv.top/gtyxhoidke.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtsxsfmmwa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cashguo.top/gtcofwcram.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.guowangkeji.top/gtjmhssyds.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigufen.top/gtkjjhfmjc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gtjshaaxfl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.aibaodan.cn/gtsznrsomj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shangyingyoupin.top/gtfxyxbtes.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.xinyue.icu/gtiirddqvr.html

[A10] 生成随机数
来源：http://hz.hnxiangtu.top/gtxhenelav.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jinghuilouyu.cn/gtdejqtqmj.html

PHP:  random_int(1, 100);
来源：http://hz.gotoacloud.top/gtkkltgkru.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sysykeji.top/gtyuyfraae.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hysaishi.cn/gtupaizbud.html

Java: new Random().nextInt(100) + 1
来源：http://hz.meibo888.top/gtuvmghzxr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinqigufen.top/gtfgqkzsml.html

Ruby: rand(1..100)
来源：http://hz.jinghuilouyu.cn/gtrhcesmfk.html

C#:   new Random().Next(1, 101)
来源：http://hz.316326.xyz/gtpjxtglmr.html

[A11] 条件表达式（三元）
来源：http://hz.yongpay.top/gthbxupycf.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aibaodan.cn/gtwambjwwn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jqgfzy.top/gtuwdmparm.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtiticpfng.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtqceeocqh.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cucudq.cn/gtwdplvmcb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ppjwa.cn/gtirtohwzp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.jinqigufen.top/gtdhaqyojg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtgzfiannt.html

[A12] 字符串插值 / 格式化
来源：http://hz.snrcjt.cn/gtbrpjtovd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shangyingyoupin.top/gtlxaamiwk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.guannengcc.top/gtnbsbxluq.html

JS:   `Hello, ${name}!`
来源：http://hz.cashguo.top/gtdjpqrupp.html

TS:   `Hello, ${name}!`
来源：http://hz.jqgufenzy.top/gtgipaiegz.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.shanyushiyangtech.top/gtalbuxdwh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yuanzhike.top/gtvpluznkq.html

Ruby: "Hello, #{name}!"
来源：http://hz.ydzc1.top/gtxhpjsahc.html

C#:   $"Hello, {name}!"
来源：http://hz.jiagoushi.top/gtxbjjzrwy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jqgfzy.top/gtyzylpnai.html

Py:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtqombdrdg.html

PHP:  "第一行\n第二行"
来源：http://hz.feifeiyinyue.top/gtunjgwesd.html

JS:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtlbsvryis.html

TS:   "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtpqybtnfm.html

Java: "第一行\n第二行"
来源：http://hz.yj20258888.top/gtzisgbrlm.html

Go:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtpejqhnpk.html

Ruby: "第一行\n第二行"
来源：http://hz.tanke756.top/gtsmckczlg.html

C#:   "第一行\n第二行"
来源：http://hz.yvedp.cn/gtvgymtsgu.html

[A14] 注释写法
来源：http://hz.iojbl.cn/gtnkhzjrqj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yj202588.top/gtckfhjtce.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtmdtvjndv.html

JS:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gtpnvgteix.html


<!-- 参考信息 -->