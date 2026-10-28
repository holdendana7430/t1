代发 wailian999

[U87] JS：解构默认值
来源：http://hz.yuxming.cn/gtmdnhktge.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenjidiqi.icu/gtlslfbbwd.html

[U88] JS：对象展开合并
来源：http://hz.xylfe.cn/gtacpwzbno.html

{ ...a, ...b }
来源：http://hz.snrcjt.cn/gtvwyuqhnd.html

[U89] JS：数组去重
来源：http://hz.chenlongwang.top/gtmvitdrkz.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtmjpovedm.html

[U90] JS：数字数组排序
来源：http://hz.birdmap.top/gtpieiepgz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtgnfvthhv.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtztdqgjyr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sweek.top/gtaoppdbnb.html

[U92] JS：深拷贝
来源：http://hz.ydjk.org.cn/gtlpapmyvg.html

structuredClone(obj)
来源：http://hz.andypj.xyz/gtaxvxwocu.html

[U93] JS：模板字符串
来源：http://hz.tianlin.xyz/gtjccuvqdg.html

`共 ${n} 条`
来源：http://hz.jlsjyb.cn/gtfttsamsf.html

[U94] JS：箭头函数
来源：http://hz.zhoulong.xyz/gtqtnwjnzl.html

const double = x => x * 2;
来源：http://hz.pengpengdd.cyou/gtlnwoxmkw.html

[U95] JS：Promise 包装
来源：http://hz.zhongyouzk.top/gtcxradwno.html

new Promise((resolve, reject) => {})
来源：http://hz.gotoacloud.top/gtxfxkdtfk.html

[U96] JS：async/await 与异常
来源：http://hz.nanxinkj.top/gtnedmornq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtwlnlmben.html

[U97] JS：并发请求
来源：http://hz.zhijiandao.cn/gtwnlxghlp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtioneyerx.html

[U98] JS：fetch 带 JSON
来源：http://hz.cheryme.top/gtkyxmyrca.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shzxlz.cn/gthswzogdc.html

[U99] JS：事件监听
来源：http://hz.yuanzhike.top/gtfeezyovg.html

el.addEventListener("click", e => {})
来源：http://hz.fengsongda.top/gtalypkugm.html

[U100] JS：DOM 查询
来源：http://hz.dashuyun.cn/gtcrqwswoz.html

document.querySelector(".item")
来源：http://hz.cashguo.top/gttskaytkd.html

[U101] JS：classList 操作
来源：http://hz.guowangkeji.top/gtejkpjlji.html

el.classList.toggle("active")
来源：http://hz.snrcjt.cn/gtcvxfziok.html

[U102] JS：本地存储
来源：http://hz.dianchejie.cn/gthfcofavo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258888.top/gtfszbkwms.html

[U103] JS：定时器
来源：http://hz.zhoulong.xyz/gtkczoxfus.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daxiang520.top/gtmuzloalz.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gtzpvfjgon.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtkykybseg.html

[U105] JS：节流
来源：http://hz.yj20258.top/gtopblmtvs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtrqqgguis.html

[U106] JS：日期格式化
来源：http://hz.nwbrower.top/gtphmhaqdz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gtjhiykksu.html

[U107] JS：数字千分位
来源：http://hz.hfpthk.cn/gtaaeoevab.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hysaishi.cn/gtyoimnxyv.html

[U108] JS：随机整数
来源：http://hz.yuxming.cn/gtuftieyoy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cheryme.top/gtogxcqpcw.html

[U109] JS：数组分组
来源：http://hz.haohaochexian.top/gtaatdmzor.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtfoqasynf.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtqrxceper.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.daria6918.cn/gtbdfztzis.html

[U111] JS：对象转 Map
来源：http://hz.316326.xyz/gtmfiipjap.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtzrcehkne.html

[U112] JS：字符串补位
来源：http://hz.zhiwuduotai.top/gtqccgpzjw.html

"7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtefpcmumn.html

[U113] JS：正则替换全部
来源：http://hz.guowangkeji.top/gtrxvgddkk.html

s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtiskvoatc.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtcqdhbxtp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhoulong.xyz/gtoxdktkbd.html

[U115] JS：生成 UUID
来源：http://hz.fzhhl.top/gtvinnjodb.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gtzveewint.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sxryk.cn/gtoxuluwvf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtnykcrwyl.html

[U117] JS：单元测试
来源：http://hz.chenjidiqi.icu/gtlmabjmkv.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gtrfqyqasu.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtiqwvlryl.html

npm i -D vite;  npx vite
来源：http://hz.redwolf501.top/gtbikswfwz.html

[U119] JS：生产构建
来源：http://hz.xziqi.cn/gtppyrtmom.html

npx vite build
来源：http://hz.smart0.xyz/gtosvsimpb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.wangdashe.top/gtkewwkfol.html

import.meta.env.VITE_API_URL
来源：http://hz.wangdashe.top/gtrukiufla.html

================================================================================
来源：http://hz.ppjwa.cn/gtyqunfjpr.html

统计汇总
来源：http://hz.tianlin.xyz/gtqxodliuv.html

================================================================================
来源：http://hz.yj20258888.top/gtyncypklh.html

按语言统计（条）：
来源：http://hz.zhixingplan.top/gtyilhgoej.html

Python ......... 252
来源：http://hz.yangfankeji.com/gtmjdippub.html

PHP ............ 252
来源：http://hz.hysaishi.cn/gteemmacsm.html

JavaScript ..... 252
来源：http://hz.c1oappe.top/gteyrafcou.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gtvahmuxbg.html

Java ........... 212
来源：http://hz.ppjwa.cn/gtihzkgqun.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtgqtvynuv.html

Ruby ........... 212
来源：http://hz.shuidangran.top/gtgrbuloet.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtjdspzvbz.html

C .............. 30
来源：http://hz.ydjk.org.cn/gtjdaylixv.html

C++ ............ 30
来源：http://hz.wangshuangyany.cn/gtppfjebil.html

SQL ............ 90
来源：http://hz.bjfxy.top/gtisejikig.html

Bash ........... 80
来源：http://hz.iojbl.cn/gtegqcddci.html

Kotlin ......... 15
来源：http://hz.jlsjyb.cn/gtmvmwxadc.html

Swift .......... 15
来源：http://hz.gzhubu.top/gtuuuldycp.html

Lua ............ 10
来源：http://hz.xziqi.cn/gtuqmcppfu.html

Perl ........... 10
来源：http://hz.mhx1999.top/gtrcwvbvxs.html

Scala .......... 10
来源：http://hz.andypj.xyz/gtswfafxzp.html

------------------------------------
来源：http://hz.zdqjudy.top/gtvsyszkbw.html

合计 ........... 2106 条
来源：http://hz.9152youxi.cn/gtihnxpnak.html

按章节统计：
来源：http://hz.tianlin.xyz/gtnajxmxid.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtrtkgyfmn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtcllhkerc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtsxshhian.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtxvukxnwk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.c1oappe.top/gtjjuwalgj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtblejkjqd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtdkaxzwsf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtyzrokfgi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtxslphpse.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gogol.net.cn/gtprjntskq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtlisnchlq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gttuprrhnh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtaugxfecb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gtpatoexgw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.52xcode.cn/gthdezesqz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtshrjltxa.html

Q SQL 专题                              90
来源：http://hz.zhaomingkeji.xyz/gtevoddftg.html

R Bash 专题                             80
来源：http://hz.jqgufenzy.top/gtnvzfxkgj.html

S C / C++ 专题                          60
来源：http://hz.yvedp.cn/gtmoiyesek.html

T 其他语言补充                          60
来源：http://hz.nanxinkj.top/gtyvvcqynm.html

U 高频实用片段                         120
来源：http://hz.hnqzz.top/gtzwiwdekz.html

------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtjpzzdnco.html

合计                                  2106 条
来源：http://hz.hnxiangtu.top/gtdfbabssm.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtssehtrae.html

使用提醒
来源：http://hz.yuxming.cn/gtctrqqjlo.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtqamvedzf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangdashe.top/gtroflrexv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shangyingyoupin.top/gtjthyzemx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtbyuhmyls.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shanyushiyangtech.top/gtwkxxqmbz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zycfv.cn/gtrvrfgurj.html

—— 文件结束 ——
来源：http://hz.zhiwuduotai.top/gtdfcrngrj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtuhnrqqyb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhiwuduotai.top/gthiwumslg.html

Common Programming Examples Cheat Book
来源：http://hz.xziqi.cn/gtkasxhtcp.html

================================================================================
来源：http://hz.ivvv.top/gtnowsnwib.html

【收录内容】
来源：http://hz.hysaishi.cn/gtravhwewc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tian-w.cn/gtavmbfiop.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydzc1.top/gtzqlksqvi.html

SQL · Bash · C · C++
来源：http://hz.yongpay.top/gtpoyxkfnu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.mhx1999.top/gtnypfpcbt.html

【使用说明】
来源：http://hz.wangshuangyany.cn/gtjihyllke.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.andypj.xyz/gtxqqunvgb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.fzhhl.top/gtohjkbtlu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxinkj.top/gtqpbbzufm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pengpengdd.cyou/gtfnvalhqm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtgajjrfaf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhaomingkeji.xyz/gtmjnopbwh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shangyingyoupin.top/gtoamxqoht.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ppjwa.cn/gtdvetntuh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yanxiufei.cn/gtqjicalgb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinqigufen.top/gtkhadulgk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnxiangtu.top/gtmfdgqcjp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenlongwang.top/gtoazmfsdq.html

【文件统计】
来源：http://hz.cheryme.top/gtxecndpmo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj202588.top/gtzwunfqfy.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtgartgaco.html

目  录
来源：http://hz.316326.xyz/gtmycjlddy.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtolurzzry.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.sxryk.cn/gtqrhyjksc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtvvzbjgcu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtgdmhhbes.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yueranfly.top/gtlujzlehm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yangfankeji.com/gtjbsbthys.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ehwqpu.com/gtiboyoqdw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ybcxt.top/gtkzgqpxwq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ppjwa.cn/gtshbutgtx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gthcoobbdu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yvedp.cn/gtdaczeosa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtfpcftjii.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtyuuzambd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtcgjxafwm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtkvosjvik.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yonumen.top/gtpzxqrauv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtbhbodgwf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hnxiangtu.top/gttsihnlbl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.c1oappe.top/gtecpkxchh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yvedp.cn/gtzswgbuug.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daria6918.cn/gtpbvlsaio.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtoyfawkpt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzbycdwvu.html

A. 基础语法与类型
来源：http://hz.pengpengdd.cyou/gtluwokzra.html

================================================================================
来源：http://hz.yj202588.top/gtyckrthop.html

[A01] Hello World
来源：http://hz.chenjidiqi.icu/gtkzdhkyid.html

Py:   print("Hello, World!")
来源：http://hz.cdnleiting.top/gtvhwcefvd.html

PHP:  echo "Hello, World!";
来源：http://hz.wangshuangyany.cn/gtjoxicywb.html

JS:   console.log("Hello, World!");
来源：http://hz.xingfuxueyuan.xyz/gtwlckwigr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gogol.net.cn/gtikgsbxuo.html

Java: System.out.println("Hello, World!");
来源：http://hz.yonumen.top/gtrjbbdpbx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.fzhhl.top/gtyumlrnsg.html

Ruby: puts "Hello, World!"
来源：http://hz.tianlin.xyz/gtbprmdeuo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtaggrxypp.html

[A02] 变量声明与赋值
来源：http://hz.zhoulong.xyz/gtroyxyely.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ywan-chungtsiang.top/gtiqgwolbt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jlsjyb.cn/gtaxexurjh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hysaishi.cn/gtjkrptpye.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hnqzz.top/gtvaqvpdne.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.feifeiyinyue.top/gtdyttviim.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgufenzy.top/gtpcdsuven.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gtndndqlay.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtpuawlzdm.html

[A03] 常量定义
来源：http://hz.yj202588.top/gtwqtxvsmt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.meibo888.top/gtfnafjple.html

PHP:  const PI = 3.14159;
来源：http://hz.andypj.xyz/gtlgdxchdw.html

JS:   const PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtbcajuyuk.html

TS:   const PI: number = 3.14159;
来源：http://hz.shuidangran.top/gtxfmujfon.html

Java: static final double PI = 3.14159;
来源：http://hz.xuanzx.com/gtnpivpmcy.html

Go:   const PI = 3.14159
来源：http://hz.jlsjyb.cn/gtbtgprryv.html

Ruby: PI = 3.14159
来源：http://hz.pengpengdd.cyou/gtaizdjvok.html

C#:   const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtuetgkrhj.html

[A04] 判断变量类型
来源：http://hz.yj20258.top/gtemdfqmza.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.quarkkingdee.top/gtfttjqxki.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dianchejie.cn/gtrdtmbvrk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cdnleiting.top/gtoswwatoe.html

TS:   typeof x; x instanceof Date
来源：http://hz.0kj1m.cn/gtukfuulnx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhijiandao.cn/gtivahvbnz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhixingplan.top/gtkbisclmc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jyoumei.cn/gtpgkcwllz.html

C#:   x.GetType().Name; x is int
来源：http://hz.tian-w.cn/gtpbqunngb.html

[A05] 整数除法与取模
来源：http://hz.jqgfzy.top/gtezohwckq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.smart0.xyz/gtrcdfknft.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aibaodan.cn/gtmttcjtwr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sweek.top/gtzlwvephu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtukzhsexl.html

Java: 7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtsohyuzpl.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtrdskxsin.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtluhijyss.html

C#:   7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gttycftajw.html

[A06] 字符串转数字
来源：http://hz.guannengcc.top/gtiyfeocdy.html

Py:   int("42"); float("3.14")
来源：http://hz.daria6918.cn/gtewnjbyyu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhijiandao.cn/gtvgojijvr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.bjfxy.top/gttcauhwse.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yuxming.cn/gtmcuxsvaf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yvedp.cn/gtyeugnorc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.feifeiyinyue.top/gtnzyfkjjg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xingfuxueyuan.xyz/gtudwfratt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pycfn.com/gtxppvpgno.html

[A07] 数字转字符串
来源：http://hz.hywenlv.cn/gthaddyvug.html

Py:   str(42)
来源：http://hz.zhengqikj.top/gtfgeilvhr.html

PHP:  (string) 42; strval(42)
来源：http://hz.hongshengwenyu.top/gtukuvtmdp.html

JS:   String(42); (42).toString()
来源：http://hz.hammf.cn/gtzjikrpfd.html

TS:   String(42)
来源：http://hz.yongpay.top/gtvpcmfkwl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.aizwys.cn/gtvcvwotrk.html

Go:   strconv.Itoa(42)
来源：http://hz.pengpengdd.cyou/gtmuglxxae.html

Ruby: 42.to_s
来源：http://hz.yvedp.cn/gtohoelwuk.html

C#:   42.ToString()
来源：http://hz.fzhhl.top/gtkxxtfytd.html

[A08] 取整与四舍五入
来源：http://hz.ivvv.top/gteoumnioh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yj20258888.top/gtcukyfnom.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yueranfly.top/gtfhgzbooz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.tianlin.xyz/gtguuifzkg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.tian-w.cn/gtppmhmvhd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtvjaqenhy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhijiandao.cn/gtmwreuiog.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jinghuilouyu.cn/gtjcczyhdv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jlsjyb.cn/gtmmqhmppn.html

[A09] 绝对值与最大最小值
来源：http://hz.chenjidiqi.icu/gttowpnzyr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hongshengwenyu.top/gtcvvuoauo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtscerzrca.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jinqigufen.top/gtjahqxsrc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtqxumaxkh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jyoumei.cn/gtpvizuxrc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.xziqi.cn/gtazspwkdf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zycfv.cn/gtabacnjqp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shzxlz.cn/gtqrfctfeb.html

[A10] 生成随机数
来源：http://hz.hywenlv.cn/gtxeljeckr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jqgufenzy.top/gtjqlxlhif.html

PHP:  random_int(1, 100);
来源：http://hz.hnxiangtu.top/gtczgvmhcj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.chenzaomai.com/gtxmlrqdem.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangdashe.top/gtgzdzyvux.html

Java: new Random().nextInt(100) + 1
来源：http://hz.chenzaomai.com/gtfwzeejig.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yueranfly.top/gtsmcyurgj.html

Ruby: rand(1..100)
来源：http://hz.yueranfly.top/gtlydyouzy.html

C#:   new Random().Next(1, 101)
来源：http://hz.guannengcc.top/gtbrbzcfuh.html

[A11] 条件表达式（三元）
来源：http://hz.jinyuanbaomall.cn/gtketeulkg.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.9152youxi.cn/gturtrhorv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtaedydeyp.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gthemcfhmg.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gtroxtadyd.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.dianchejie.cn/gtnfqfddyq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.pengpengdd.cyou/gtsrxllakr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtkxqlmvus.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtbvsapgop.html

[A12] 字符串插值 / 格式化
来源：http://hz.snrcjt.cn/gtealhfdzr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yanxiufei.cn/gtswhixkkr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.9152youxi.cn/gtcrwvbpzz.html

JS:   `Hello, ${name}!`
来源：http://hz.ydzc1.top/gtbmpkcxin.html

TS:   `Hello, ${name}!`
来源：http://hz.mhx1999.top/gtqlibjvxm.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yuxming.cn/gtwxonzver.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.daxiang520.top/gtfiluzkkw.html

Ruby: "Hello, #{name}!"
来源：http://hz.feifeiyinyue.top/gtiylplxue.html

C#:   $"Hello, {name}!"
来源：http://hz.xuanzx.com/gtwfmixyyf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.feifeiyinyue.top/gtdzktdyba.html

Py:   "第一行\n第二行"
来源：http://hz.yonumen.top/gtnfsewrhg.html

PHP:  "第一行\n第二行"
来源：http://hz.ybcxt.top/gtwafatzno.html

JS:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtqijmaupf.html

TS:   "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gtdlsqrzjo.html

Java: "第一行\n第二行"
来源：http://hz.xylfe.cn/gtaqkwuhnu.html

Go:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtookptmdz.html

Ruby: "第一行\n第二行"
来源：http://hz.sysykeji.top/gtazkubfxd.html

C#:   "第一行\n第二行"
来源：http://hz.wangdashe.top/gtkdtflwiv.html

[A14] 注释写法
来源：http://hz.sweek.top/gtneumufar.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.pycfn.com/gtkzfyqsof.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtcfbvrepx.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinqigufen.top/gtdlrqgcvs.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhijiandao.cn/gtapcojiod.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.birdmap.top/gtlbilvwkh.html

Go:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtbunkxtjk.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.pengpengdd.cyou/gthubhlwet.html


<!-- 参考信息 -->