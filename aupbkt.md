代发 wailian999

[U87] JS：解构默认值
来源：http://hz.hysaishi.cn/gtiorduexn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuxming.cn/gtghwrqgsn.html

[U88] JS：对象展开合并
来源：http://hz.yj20258888.top/gtnszzsqoo.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gtmmpexikt.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gtsvgcyrjr.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtbyncvzji.html

[U90] JS：数字数组排序
来源：http://hz.xuanzx.com/gtofbkzcbs.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtzxmxyljh.html

[U91] JS：对象键值遍历
来源：http://hz.316326.xyz/gtsmtqsumo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.vqdsnc.cn/gtfqunvlwd.html

[U92] JS：深拷贝
来源：http://hz.gotoacloud.top/gtziqkgrhj.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtfcvbfnxm.html

[U93] JS：模板字符串
来源：http://hz.tian-w.cn/gtkvjpdimj.html

`共 ${n} 条`
来源：http://hz.hysaishi.cn/gtjuuroiga.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gtqrcooijd.html

const double = x => x * 2;
来源：http://hz.snrcjt.cn/gtxtsfaudw.html

[U95] JS：Promise 包装
来源：http://hz.zhaomingkeji.xyz/gtewccjphk.html

new Promise((resolve, reject) => {})
来源：http://hz.yvedp.cn/gtxqxswqpx.html

[U96] JS：async/await 与异常
来源：http://hz.yongpay.top/gtzewuareq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtvwvmaatb.html

[U97] JS：并发请求
来源：http://hz.ivvv.top/gtflxlbuad.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtwhxskhbu.html

[U98] JS：fetch 带 JSON
来源：http://hz.yongpay.top/gtafpbmvyi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258888.top/gtkmtjvhpt.html

[U99] JS：事件监听
来源：http://hz.jinghuilouyu.cn/gtgspjljvy.html

el.addEventListener("click", e => {})
来源：http://hz.tanke756.top/gtwfbbatpt.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gthvpirkgv.html

document.querySelector(".item")
来源：http://hz.sysykeji.top/gtnuxitqao.html

[U101] JS：classList 操作
来源：http://hz.haohaochexian.top/gtwuoycatf.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtfuegzntq.html

[U102] JS：本地存储
来源：http://hz.c1oappe.top/gtkghhryrl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cdnleiting.top/gtamunqdaw.html

[U103] JS：定时器
来源：http://hz.zhaomingkeji.xyz/gtvjxuyeqj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtvayzbubb.html

[U104] JS：防抖
来源：http://hz.fzhhl.top/gtukjzshng.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtmttgemxr.html

[U105] JS：节流
来源：http://hz.ywan-chungtsiang.top/gtsvznylgk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj202588.top/gtruiiduzz.html

[U106] JS：日期格式化
来源：http://hz.0kj1m.cn/gtksqdaymf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gzhubu.top/gtbqdohymr.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtdnblqdcw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gogol.net.cn/gtkxmadeqn.html

[U108] JS：随机整数
来源：http://hz.hongshengwenyu.top/gtjsdcwftr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hysaishi.cn/gtgixonykz.html

[U109] JS：数组分组
来源：http://hz.xinyue.icu/gtjmmdjzqx.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gttswxluty.html

[U110] JS：数组分块
来源：http://hz.wangdashe.top/gtndlnemps.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhongyouzk.top/gtfnnejllz.html

[U111] JS：对象转 Map
来源：http://hz.daxiang520.top/gtemqaqhlr.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtfuuyumdm.html

[U112] JS：字符串补位
来源：http://hz.jqgfzy.top/gthndsnagq.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtamszgyml.html

[U113] JS：正则替换全部
来源：http://hz.yj20258888.top/gtbsoyldoz.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gttzbguiqu.html

[U114] JS：JSON 深比较
来源：http://hz.sxryk.cn/gtatvltmjn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtwptvhxlb.html

[U115] JS：生成 UUID
来源：http://hz.fengsongda.top/gtazwygknd.html

crypto.randomUUID()
来源：http://hz.c1oappe.top/gtfkangkqr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xinyue.icu/gtkonnergg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hfpthk.cn/gtowybkfot.html

[U117] JS：单元测试
来源：http://hz.wangdashe.top/gtnnvzlhch.html

npm i -D vitest;  npx vitest
来源：http://hz.gogol.net.cn/gtmbppfuwf.html

[U118] JS：开发服务器
来源：http://hz.yonumen.top/gtmepydgen.html

npm i -D vite;  npx vite
来源：http://hz.mhx1999.top/gtdvsfhwmb.html

[U119] JS：生产构建
来源：http://hz.pengpengdd.cyou/gtunphtlwp.html

npx vite build
来源：http://hz.redwolf501.top/gtnvsbylpd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gaohongyu789.top/gtixxfwqls.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtsyugitvs.html

================================================================================
来源：http://hz.shzxlz.cn/gtbwsetpyh.html

统计汇总
来源：http://hz.tian-w.cn/gtxeqrvnjn.html

================================================================================
来源：http://hz.316326.xyz/gtojhohone.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtmyypvwtz.html

Python ......... 252
来源：http://hz.316326.xyz/gtydipxdul.html

PHP ............ 252
来源：http://hz.daxiang520.top/gtaidylifg.html

JavaScript ..... 252
来源：http://hz.tian-w.cn/gtkicbuwan.html

TypeScript ..... 212
来源：http://hz.pycfn.com/gtxughlwcy.html

Java ........... 212
来源：http://hz.wangshuangyany.cn/gtvsrvaecy.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtduirsonf.html

Ruby ........... 212
来源：http://hz.316326.xyz/gtvlrcnqdf.html

C# ............. 212
来源：http://hz.hammf.cn/gtiigdzdlm.html

C .............. 30
来源：http://hz.sufxvd.cn/gtfcvighfl.html

C++ ............ 30
来源：http://hz.xuanzx.com/gtbftehrvv.html

SQL ............ 90
来源：http://hz.svipenyu.cn/gtsoxujaja.html

Bash ........... 80
来源：http://hz.feifeiyinyue.top/gtaojntocs.html

Kotlin ......... 15
来源：http://hz.yuanzhike.top/gtboaoemkf.html

Swift .......... 15
来源：http://hz.gotoacloud.top/gtxunhujvr.html

Lua ............ 10
来源：http://hz.dashuyun.cn/gtsyfdotvb.html

Perl ........... 10
来源：http://hz.nwbrower.top/gtyctimurd.html

Scala .......... 10
来源：http://hz.sweek.top/gtpdbpdlpt.html

------------------------------------
来源：http://hz.hywenlv.cn/gtdivapavy.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gtzlcpeigu.html

按章节统计：
来源：http://hz.zhixingplan.top/gtsczcgjnd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtmlgikljz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtzxjyiwfa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtwkmhkjps.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtgadhyhhq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenzaomai.com/gtzgtfjrce.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtturpwtzu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtprzfvtvj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gzhubu.top/gtwdivqpbq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtopsyybvw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtroqgskiy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtehooppwy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtrzyoyyve.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gthukememj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtibyjlzpe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gtmmajkfox.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gthjiupfjp.html

Q SQL 专题                              90
来源：http://hz.xylfe.cn/gtecipcoyc.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtrlfwkisg.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangtech.top/gtqgfnbtkd.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtqbcgzvxf.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gtmsgptkbl.html

------------------------------------
来源：http://hz.mhx1999.top/gtaclshtao.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtxwinjfyk.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtlnqncvmi.html

使用提醒
来源：http://hz.yvedp.cn/gtktiimuum.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtndxkdlza.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.snrcjt.cn/gtldkarqwz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhiwuduotai.top/gtowqvdkrh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinqigufen.top/gtdpjrqjxa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hongshengwenyu.top/gtybccxvca.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.chenzaomai.com/gtktlcbbqb.html

—— 文件结束 ——
来源：http://hz.jianghu66.top/gttpxzhbxp.html

================================================================================
来源：http://hz.nwbrower.top/gtlefqnxdn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258888.top/gtyjdzglld.html

Common Programming Examples Cheat Book
来源：http://hz.gogol.net.cn/gtgeqancyb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnyuxwgst.html

【收录内容】
来源：http://hz.chenjidiqi.icu/gtaphqqrtx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shuidangran.top/gtmmpvezsc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinqigufen.top/gtfglxxycs.html

SQL · Bash · C · C++
来源：http://hz.snrcjt.cn/gtuccxihxt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hfpthk.cn/gtikirzhgb.html

【使用说明】
来源：http://hz.wangdashe.top/gtaxgyjier.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ivvv.top/gtitaaeoqf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shangyingyoupin.top/gtdvrmbscq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gthioedsxg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtclymrfhf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgfzy.top/gtfgooftwz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.quarkkingdee.top/gtypwzgfna.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cashguo.top/gtrobikwrw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hysaishi.cn/gtpyyzbxnv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuxming.cn/gtlmqazgal.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jiagoushi.top/gtkcwahsjc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtkbtnllwr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tian-w.cn/gtqfsfewfr.html

【文件统计】
来源：http://hz.nanxinkj.top/gtyijqtfzl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhongyouzk.top/gteiwevejm.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtikuikezy.html

目  录
来源：http://hz.yuanzhike.top/gtgklzmmck.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtjhllehhg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yuanzhike.top/gtveofzypp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtcpontupk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtcaoqpqxo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtgkeejjax.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xylfe.cn/gtcfowztqo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gtlctmkatz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtcufhhvdv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtsnczeqri.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtmeoccxxi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtubmmqreg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtlnubazjs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtfnsbhiqp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtdqklooes.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.316326.xyz/gtlaatgokb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hongshengwenyu.top/gtegulaocs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtghvngtrx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yueranfly.top/gtqdlmyvsf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinghuilouyu.cn/gtrbefxsyi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtlxuumldr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtdcoqeoug.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ywan-chungtsiang.top/gtyrcsutxn.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwkpxalvg.html

A. 基础语法与类型
来源：http://hz.shanyushiyangkeji.top/gtilkehncs.html

================================================================================
来源：http://hz.fzhhl.top/gtudmswhld.html

[A01] Hello World
来源：http://hz.haohaochexian.top/gtiwvrwmkl.html

Py:   print("Hello, World!")
来源：http://hz.zhengqikj.top/gtknfkdpgq.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxinkj.top/gtxjlcgcob.html

JS:   console.log("Hello, World!");
来源：http://hz.hfpthk.cn/gtipececcr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.fzhhl.top/gtudfuicxp.html

Java: System.out.println("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtgatlboih.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xylfe.cn/gtnmzduouj.html

Ruby: puts "Hello, World!"
来源：http://hz.havefunace.top/gthyvjxuao.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.dashuyun.cn/gtxbqefcvm.html

[A02] 变量声明与赋值
来源：http://hz.cheryme.top/gtcngtjfst.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hammf.cn/gtucdqhyjs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gtgdhpkgha.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinyuanbaomall.cn/gtbpbugqxr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydjk.org.cn/gtgddbvslk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtovvvlciv.html

Go:   name := "Alex"; age := 20
来源：http://hz.ydzc1.top/gthjwqkryn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cheryme.top/gtlpjdyshg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.tanke756.top/gtexhbjgst.html

[A03] 常量定义
来源：http://hz.jinghuilouyu.cn/gtftxpeuub.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.birdmap.top/gtfkdtxuel.html

PHP:  const PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtjatthoyx.html

JS:   const PI = 3.14159;
来源：http://hz.mhx1999.top/gtlzjtakaz.html

TS:   const PI: number = 3.14159;
来源：http://hz.tanke756.top/gtlzoicoil.html

Java: static final double PI = 3.14159;
来源：http://hz.xuanzx.com/gtkmzumapg.html

Go:   const PI = 3.14159
来源：http://hz.hfpthk.cn/gtifkwmfzd.html

Ruby: PI = 3.14159
来源：http://hz.ydjk.org.cn/gtvnqkyztp.html

C#:   const double PI = 3.14159;
来源：http://hz.birdmap.top/gtbfagblod.html

[A04] 判断变量类型
来源：http://hz.chenjidiqi.icu/gtjklcrpgg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gtilzgpxtl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.mhx1999.top/gtheylqxpv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yvedp.cn/gtfoymrasf.html

TS:   typeof x; x instanceof Date
来源：http://hz.dashuyun.cn/gtqzxammiz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xuetiantiany.cn/gtebrfohua.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.0kj1m.cn/gtabzciasz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ydzc1.top/gtafwfylqx.html

C#:   x.GetType().Name; x is int
来源：http://hz.zycfv.cn/gtqvyehkpa.html

[A05] 整数除法与取模
来源：http://hz.ppjwa.cn/gtkytsjqsj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj202588.top/gtxayfrmcp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zycfv.cn/gtfeyaiojw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtoskspkqn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tanke756.top/gtwxxohxun.html

Java: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtshnuahsz.html

Go:   7 / 2; 7 % 2
来源：http://hz.9152youxi.cn/gtxpitzyvh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtokpkjksy.html

C#:   7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gtwidqdcbo.html

[A06] 字符串转数字
来源：http://hz.chenzaomai.com/gtpstiidow.html

Py:   int("42"); float("3.14")
来源：http://hz.ppjwa.cn/gtbyeqyyeo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.sufxvd.cn/gtdqwufpxy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtnpqzcfop.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jqgfzy.top/gtcfvvzlrv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.guowangkeji.top/gtssjdnvoz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gtdtfyqlzh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gotoacloud.top/gtaibkgyuo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ydzc1.top/gtzkiwxprz.html

[A07] 数字转字符串
来源：http://hz.cqqwz.cn/gtzhxytoll.html

Py:   str(42)
来源：http://hz.birdmap.top/gtbmqhxvsc.html

PHP:  (string) 42; strval(42)
来源：http://hz.cucudq.cn/gtcuwuhebf.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtddbwlnyc.html

TS:   String(42)
来源：http://hz.xingfuxueyuan.xyz/gtuaepmtgb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shzxlz.cn/gtzecmpmud.html

Go:   strconv.Itoa(42)
来源：http://hz.hammf.cn/gtqwmgzoot.html

Ruby: 42.to_s
来源：http://hz.cheryme.top/gtlnaejmkh.html

C#:   42.ToString()
来源：http://hz.shzxlz.cn/gtuixencrq.html

[A08] 取整与四舍五入
来源：http://hz.gzhubu.top/gtapgwezkq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aizwys.cn/gtmsczqbxz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yueranfly.top/gtnapxcetr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.wangdashe.top/gtncsqmhdk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigfzy.top/gtdnjyaebq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.bjfxy.top/gtnffdixta.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.gotoacloud.top/gtnugpamvb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jyoumei.cn/gtdykcnqdh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cdnleiting.top/gtdcxocmmk.html

[A09] 绝对值与最大最小值
来源：http://hz.zycfv.cn/gteebixizc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuxming.cn/gtttbgpirz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nwbrower.top/gtdxjxhcrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.9152youxi.cn/gtlkdrbigv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.pengpengdd.cyou/gtpkdxonrc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hongshengwenyu.top/gtpjqnxnjh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.meibo888.top/gtwilfagnk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jiagoushi.top/gtpplzwbvs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shuidangran.top/gtoqotexxq.html

[A10] 生成随机数
来源：http://hz.snrcjt.cn/gtxdlkoajb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.gzhubu.top/gtakfzsqmj.html

PHP:  random_int(1, 100);
来源：http://hz.aibaodan.cn/gttiahnplj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ywan-chungtsiang.top/gtveyirhic.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gzhubu.top/gthqajubln.html

Java: new Random().nextInt(100) + 1
来源：http://hz.mhx1999.top/gtpayrkpmz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.pengpengdd.cyou/gtslcoonzr.html

Ruby: rand(1..100)
来源：http://hz.pycfn.com/gtgiejqxre.html

C#:   new Random().Next(1, 101)
来源：http://hz.jqgfzy.top/gtssjmtwli.html

[A11] 条件表达式（三元）
来源：http://hz.sweek.top/gtbtzvyiar.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhaomingkeji.xyz/gtmhmluhxx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtfgkjbgsz.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtyqgpwbws.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gtkrvyuzku.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtodhmbqxb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.dashuyun.cn/gtnnfohsqb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtpwuxlyig.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtgvuuafdy.html

[A12] 字符串插值 / 格式化
来源：http://hz.cdnleiting.top/gtzfdipays.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.chenjidiqi.icu/gtasjiehgd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.0kj1m.cn/gtzlogiegg.html

JS:   `Hello, ${name}!`
来源：http://hz.shuidangran.top/gtsfapndrl.html

TS:   `Hello, ${name}!`
来源：http://hz.pycfn.com/gtpqsaxixt.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhaomingkeji.xyz/gtrlfnszst.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.c1oappe.top/gtkrbwacwx.html

Ruby: "Hello, #{name}!"
来源：http://hz.haohaochexian.top/gtnvtmmcbi.html

C#:   $"Hello, {name}!"
来源：http://hz.xziqi.cn/gtniuvhobw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ivvv.top/gtwlvzhijk.html

Py:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtbunricug.html

PHP:  "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtzahbijmc.html

JS:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gtgjnkkccq.html

TS:   "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtziwvpccy.html

Java: "第一行\n第二行"
来源：http://hz.ydzc1.top/gtxfqjbtwn.html

Go:   "第一行\n第二行"
来源：http://hz.vqdsnc.cn/gtxmyiqcvi.html

Ruby: "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtohuizgwh.html

C#:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtjxaxhpgl.html

[A14] 注释写法
来源：http://hz.hongshengwenyu.top/gtmkknzcxy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.shzxlz.cn/gttymynwfu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtttadkscd.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtggilaesj.html

TS:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gtxwoulvlh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sysykeji.top/gtgqpfervj.html

Go:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtisfjcdhl.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhixingplan.top/gtxsqjrrvs.html


<!-- 参考信息 -->