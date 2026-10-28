代发 wailian999

[U89] JS：数组去重
来源：http://hz.svipenyu.cn/gtpdfyuate.html

[...new Set(arr)]
来源：http://hz.chenlongwang.top/gtwsivmehr.html

[U90] JS：数字数组排序
来源：http://hz.iojbl.cn/gtblrifhum.html

[...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtkbbtmlqn.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangkeji.top/gthfttqzxy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.c1oappe.top/gtklfxjleu.html

[U92] JS：深拷贝
来源：http://hz.wangshuangyany.cn/gtewwwonrq.html

structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtgyehiqrx.html

[U93] JS：模板字符串
来源：http://hz.fengsongda.top/gtlsqtrhya.html

`共 ${n} 条`
来源：http://hz.jqgufenzy.top/gtbajveiqj.html

[U94] JS：箭头函数
来源：http://hz.sxryk.cn/gtnlwrwhfo.html

const double = x => x * 2;
来源：http://hz.zhengqikj.top/gtndrpqbdg.html

[U95] JS：Promise 包装
来源：http://hz.meibo888.top/gtphleryrw.html

new Promise((resolve, reject) => {})
来源：http://hz.yuanzhike.top/gtidfivgft.html

[U96] JS：async/await 与异常
来源：http://hz.guannengcc.top/gtvoqqspga.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtnrmkxhzp.html

[U97] JS：并发请求
来源：http://hz.shuidangran.top/gtvweygslv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtooubbbjc.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenjidiqi.icu/gtcvklnbzc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.meibo888.top/gthuhpjgni.html

[U99] JS：事件监听
来源：http://hz.zhongyouzk.top/gtrdxgpqwu.html

el.addEventListener("click", e => {})
来源：http://hz.xingfuxueyuan.xyz/gthpwkwhgr.html

[U100] JS：DOM 查询
来源：http://hz.jianghu66.top/gtbnxyqehj.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtqgppmsmc.html

[U101] JS：classList 操作
来源：http://hz.cheryme.top/gtwepixmhw.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtzmvdpoil.html

[U102] JS：本地存储
来源：http://hz.xziqi.cn/gtmanponsn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gogol.net.cn/gtryaiiheb.html

[U103] JS：定时器
来源：http://hz.jinqigfzy.top/gtnkxzaagw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigufen.top/gtfnhdmdgv.html

[U104] JS：防抖
来源：http://hz.wangshuangyany.cn/gtelczvovl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtwzhpwumn.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtgfyktjix.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinyuanbaomall.cn/gtekvwsapx.html

[U106] JS：日期格式化
来源：http://hz.yuxming.cn/gtztilcgev.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jyoumei.cn/gtbjigxapt.html

[U107] JS：数字千分位
来源：http://hz.pycfn.com/gtvyjixxxh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.snrcjt.cn/gthqyaunwg.html

[U108] JS：随机整数
来源：http://hz.mhx1999.top/gtphstfjvh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hywenlv.cn/gtrsfajctx.html

[U109] JS：数组分组
来源：http://hz.jinghuilouyu.cn/gtdkozhtuu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtxgqpbxqa.html

[U110] JS：数组分块
来源：http://hz.yonumen.top/gtrzvpzxvc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtrlzthzku.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtxrgtptkc.html

new Map(Object.entries(obj))
来源：http://hz.ivvv.top/gthbrkygdb.html

[U112] JS：字符串补位
来源：http://hz.jinqigufen.top/gtmokznvja.html

"7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtjkdmrwjj.html

[U113] JS：正则替换全部
来源：http://hz.xziqi.cn/gtizmixhxg.html

s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtbaqhobca.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigufen.top/gtyhaskezz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtozrmytuf.html

[U115] JS：生成 UUID
来源：http://hz.chenjidiqi.icu/gtdngcehsb.html

crypto.randomUUID()
来源：http://hz.jinqigufen.top/gthnxtehpr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gtaiueuxnq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cucudq.cn/gtmcidtbbk.html

[U117] JS：单元测试
来源：http://hz.sufxvd.cn/gtncfuwuzl.html

npm i -D vitest;  npx vitest
来源：http://hz.sxryk.cn/gtesnfegdp.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtbosexfpy.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtdfpjelft.html

[U119] JS：生产构建
来源：http://hz.xylfe.cn/gtkqzvgkxh.html

npx vite build
来源：http://hz.haohaochexian.top/gtcjzbwwvd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtnmhgfoxy.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtossjzmdk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdcqyjkpf.html

统计汇总
来源：http://hz.xylfe.cn/gtvnsvziap.html

================================================================================
来源：http://hz.iojbl.cn/gtsfwxqcid.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtlwtewdvv.html

Python ......... 252
来源：http://hz.jinghuilouyu.cn/gtoedtbyde.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtxeytlmjj.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gthfcfwspi.html

TypeScript ..... 212
来源：http://hz.havefunace.top/gtdzyotwqb.html

Java ........... 212
来源：http://hz.xuetiantiany.cn/gtywztkmxj.html

Go ............. 212
来源：http://hz.yonumen.top/gtyuyeqdub.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gterffgyjh.html

C# ............. 212
来源：http://hz.chenlongwang.top/gtlggtpogx.html

C .............. 30
来源：http://hz.cucudq.cn/gteiehjasx.html

C++ ............ 30
来源：http://hz.wangdashe.top/gtcrgfvjso.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gtulgzwgyp.html

Bash ........... 80
来源：http://hz.vqdsnc.cn/gtappeejug.html

Kotlin ......... 15
来源：http://hz.jinqigufen.top/gtvzssvosp.html

Swift .......... 15
来源：http://hz.zhijiandao.cn/gtttpzfshx.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtkncjteao.html

Perl ........... 10
来源：http://hz.dianchejie.cn/gtvioswqze.html

Scala .......... 10
来源：http://hz.ydzc1.top/gtokuydaos.html

------------------------------------
来源：http://hz.zdqjudy.top/gtnwambpzy.html

合计 ........... 2106 条
来源：http://hz.shuidangran.top/gttejewumy.html

按章节统计：
来源：http://hz.jqgufenzy.top/gtnsgwgjha.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtlkkibnkc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtdrqyukaj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtfadhzejp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtnivcrgeh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yongpay.top/gtbljtlecs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gtisassjqx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtfbzatovt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jinyuanbaomall.cn/gtxtwtnzpc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtdpfcbyal.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtvblgwopi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gthxqlybbp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtsiewaxfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtjrjzzmmu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.tanke756.top/gtenfpryxd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.mhx1999.top/gtqplrzfum.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtglbkaoxp.html

Q SQL 专题                              90
来源：http://hz.0kj1m.cn/gthglyuuuc.html

R Bash 专题                             80
来源：http://hz.jyoumei.cn/gtvjodlfoe.html

S C / C++ 专题                          60
来源：http://hz.ivvv.top/gthouzahdk.html

T 其他语言补充                          60
来源：http://hz.shzxlz.cn/gtndqxztsj.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtjtayjtgx.html

------------------------------------
来源：http://hz.redwolf501.top/gtqrlaphfx.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtnusadmnr.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtotlehdqi.html

使用提醒
来源：http://hz.redwolf501.top/gtrjsklpxe.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtwtdurjll.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yvedp.cn/gtdxraocnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jqgufenzy.top/gtbhzmfngg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ybcxt.top/gtomhustax.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.meibo888.top/gtbslhhmtj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fzhhl.top/gtbfigfnvg.html

—— 文件结束 ——
来源：http://hz.316326.xyz/gtadajzqtn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzfnyidtz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tianlin.xyz/gtmckdaqic.html

Common Programming Examples Cheat Book
来源：http://hz.zdqjudy.top/gteowosyai.html

================================================================================
来源：http://hz.sxryk.cn/gtyslcihbb.html

【收录内容】
来源：http://hz.tian-w.cn/gttgdryydy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sxryk.cn/gtcuysnzbh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.wangshuangyany.cn/gtyjwmgspr.html

SQL · Bash · C · C++
来源：http://hz.hnqzz.top/gtcckeliew.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cucudq.cn/gtgusfjjgo.html

【使用说明】
来源：http://hz.jinqigufen.top/gtzgkagptg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xinyue.icu/gtqkrpjmkp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nanxuanxn.top/gtywsevbwn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.wangshuangyany.cn/gtxvmlazub.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtuznwolmt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gotoacloud.top/gtlkuiwgwx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258888.top/gtkzvsibbd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yonumen.top/gtrynkifso.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hysaishi.cn/gttqlfkrqj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xziqi.cn/gtllpwleji.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jlsjyb.cn/gtvcxgaast.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ivvv.top/gtfvnsfqxf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangshuangyany.cn/gtoyxcfixv.html

【文件统计】
来源：http://hz.ehwqpu.com/gtwcfodvkb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.meibo888.top/gtztfslxfe.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gtfkypvfbe.html

目  录
来源：http://hz.yuanzhike.top/gtcezziozu.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gthqxloegt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hnqzz.top/gtrvudqpjf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtiwpvfspo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtowueczzl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtifkluzxh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtsxcznffq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtdagfjizl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtyrcgrhqn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtagqhnsdx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtaygodlgw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtvmwueggi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtdjocejzy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtvanjajqt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtwzfqgpfm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hongshengwenyu.top/gtyzqbdfzq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.316326.xyz/gtzzobpyoz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtlehpecec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jqgfzy.top/gtuafqcqzs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fzhhl.top/gtpexrbhgr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hywenlv.cn/gtyvqzlmst.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtyonwmblu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.meibo888.top/gtnzomximz.html

================================================================================
来源：http://hz.gotoacloud.top/gtqcwrqhpd.html

A. 基础语法与类型
来源：http://hz.aibaodan.cn/gtdocmdvlb.html

================================================================================
来源：http://hz.shzxlz.cn/gtmzzsdsrt.html

[A01] Hello World
来源：http://hz.sufxvd.cn/gtndbqsbov.html

Py:   print("Hello, World!")
来源：http://hz.yj202588.top/gtlwaxnyln.html

PHP:  echo "Hello, World!";
来源：http://hz.ydjk.org.cn/gtmkvzfuom.html

JS:   console.log("Hello, World!");
来源：http://hz.cheryme.top/gtdkgntviv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xingfuxueyuan.xyz/gtytdjvtfh.html

Java: System.out.println("Hello, World!");
来源：http://hz.52xcode.cn/gtkidcektr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xuanzx.com/gtlmptjart.html

Ruby: puts "Hello, World!"
来源：http://hz.feifeiyinyue.top/gtxzizjssq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.pycfn.com/gtxgvgkqif.html

[A02] 变量声明与赋值
来源：http://hz.zycfv.cn/gtdjkuueiu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ehwqpu.com/gtjzreucdg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zdqjudy.top/gtdotwfbrl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj202588.top/gtneecvknw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hongshengwenyu.top/gtmkelsmii.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.quarkkingdee.top/gtojwfbfrg.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhengqikj.top/gthfckpxrs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.haohaochexian.top/gtfvmenfri.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhixingplan.top/gtntgoxyco.html

[A03] 常量定义
来源：http://hz.zhixingplan.top/gtotxxjqmg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xingfuxueyuan.xyz/gtnqzyldtj.html

PHP:  const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtpwnrauut.html

JS:   const PI = 3.14159;
来源：http://hz.cheryme.top/gtabufrjtk.html

TS:   const PI: number = 3.14159;
来源：http://hz.sufxvd.cn/gtvgzvedcu.html

Java: static final double PI = 3.14159;
来源：http://hz.cucudq.cn/gtdljlsazy.html

Go:   const PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtrxcqaibu.html

Ruby: PI = 3.14159
来源：http://hz.hywenlv.cn/gtxfrycwaf.html

C#:   const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtmdwuqisp.html

[A04] 判断变量类型
来源：http://hz.svipenyu.cn/gtpydqcyuy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinyuanbaomall.cn/gtwjpbnunm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.birdmap.top/gtcuzhzkqy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.andypj.xyz/gtknrfcfqr.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhixingplan.top/gtwfppjcsh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gtqxwhdfjg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zycfv.cn/gtpizqdtkg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shuidangran.top/gtywanasth.html

C#:   x.GetType().Name; x is int
来源：http://hz.zycfv.cn/gtgtjwngdc.html

[A05] 整数除法与取模
来源：http://hz.jinqigufen.top/gtudgjxvwp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yanxiufei.cn/gtlepmkefr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yongpay.top/gtbcdvypnv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtyucvlbdw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hysaishi.cn/gtreoqgufr.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtzrbdmkin.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtkdcswmqs.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gttapnpvgm.html

C#:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtlmithkse.html

[A06] 字符串转数字
来源：http://hz.gogol.net.cn/gtzanvkhld.html

Py:   int("42"); float("3.14")
来源：http://hz.aizwys.cn/gtwkelrdov.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daria6918.cn/gtiroerkfv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.haohaochexian.top/gtgexoatep.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.havefunace.top/gtifadkjpd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.redwolf501.top/gttabbinog.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yj20258.top/gtsqogfskm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ppjwa.cn/gtpjgnkmyc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hammf.cn/gtadrlblzr.html

[A07] 数字转字符串
来源：http://hz.xingfuxueyuan.xyz/gtgczhkzop.html

Py:   str(42)
来源：http://hz.ivvv.top/gtwvkmejuk.html

PHP:  (string) 42; strval(42)
来源：http://hz.ehwqpu.com/gtspcwyyqm.html

JS:   String(42); (42).toString()
来源：http://hz.daria6918.cn/gthhbsxqjw.html

TS:   String(42)
来源：http://hz.yvedp.cn/gtctuyljwb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hywenlv.cn/gttbjqtobq.html

Go:   strconv.Itoa(42)
来源：http://hz.ydzc1.top/gtbrlxcvjd.html

Ruby: 42.to_s
来源：http://hz.aibaodan.cn/gtjtpzwjea.html

C#:   42.ToString()
来源：http://hz.ehwqpu.com/gtrlfvmror.html

[A08] 取整与四舍五入
来源：http://hz.xingfuxueyuan.xyz/gtbvjenowd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.guowangkeji.top/gtphnpaght.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.vqdsnc.cn/gtyirvqnqc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.smart0.xyz/gtrmjeveip.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.daxiang520.top/gttohkdgxk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xziqi.cn/gttnobikqs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hfpthk.cn/gtdgtdxwqe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yuanzhike.top/gtzdxxqbsc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtmkiylxyd.html

[A09] 绝对值与最大最小值
来源：http://hz.ydjk.org.cn/gtlenvlgyq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xziqi.cn/gtgdcdlsqu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhongyouzk.top/gtqstdazhn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.svipenyu.cn/gtgzxiephu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.sweek.top/gtwhqsecco.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xinyue.icu/gthlvngecw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hnxiangtu.top/gtplrmsysq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xylfe.cn/gtvbmqfzfn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yonumen.top/gtkpsclpyx.html

[A10] 生成随机数
来源：http://hz.zhixingplan.top/gtyxevppxb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yj20258888.top/gtguoolaxb.html

PHP:  random_int(1, 100);
来源：http://hz.shuidangran.top/gtjrnhmyvo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhijiandao.cn/gtrwayynlu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yongpay.top/gtkzeqwexu.html

Java: new Random().nextInt(100) + 1
来源：http://hz.shanyushiyangtech.top/gtaoynjmbd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.tian-w.cn/gtnrbbawia.html

Ruby: rand(1..100)
来源：http://hz.yonumen.top/gtdxajncnt.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj20258888.top/gtocuuhexj.html

[A11] 条件表达式（三元）
来源：http://hz.shzxlz.cn/gtvsytxvpv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.quarkkingdee.top/gtukyqexzr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gteuhxoyfx.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtsizswbwm.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.nanxuanxn.top/gtnmuqhgmy.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtufdsjipm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.meibo888.top/gtgggyhcmz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.svipenyu.cn/gtjbruzpnw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.nanxuanxn.top/gtezyjvqbr.html

[A12] 字符串插值 / 格式化
来源：http://hz.redwolf501.top/gtjiejgcdb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jqgfzy.top/gtnfgddnwk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.chenzaomai.com/gtahmhjawq.html

JS:   `Hello, ${name}!`
来源：http://hz.ppjwa.cn/gtcykamdug.html

TS:   `Hello, ${name}!`
来源：http://hz.quarkkingdee.top/gtwjdexauy.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hysaishi.cn/gtcbviszpf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hfpthk.cn/gtpujtgnba.html

Ruby: "Hello, #{name}!"
来源：http://hz.svipenyu.cn/gtjvxjorma.html

C#:   $"Hello, {name}!"
来源：http://hz.yj202588.top/gtyqspipcn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xingfuxueyuan.xyz/gtkkjhsltd.html

Py:   "第一行\n第二行"
来源：http://hz.wangshuangyany.cn/gtohjrksks.html

PHP:  "第一行\n第二行"
来源：http://hz.52xcode.cn/gtqihurkrv.html

JS:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtreiqejeq.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtimwjvotk.html

Java: "第一行\n第二行"
来源：http://hz.daxiang520.top/gtxrybanzq.html

Go:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtdhogrzpo.html

Ruby: "第一行\n第二行"
来源：http://hz.ydzc1.top/gtpyfctphi.html

C#:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtcqnxpdcn.html

[A14] 注释写法
来源：http://hz.haohaochexian.top/gtswwqtftm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.bjfxy.top/gtbowpjwhe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtovkzglge.html

JS:   // 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtuwilfege.html

TS:   // 单行；/* 多行 */
来源：http://hz.yj20258.top/gthdittelj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhongyouzk.top/gtkykuebqj.html

Go:   // 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtmknmecfy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yanxiufei.cn/gtlyxhtcxc.html

C#:   // 单行；/* 多行 */
来源：http://hz.jinyuanbaomall.cn/gtaqhyontm.html

[A15] 空值判断与默认值
来源：http://hz.52xcode.cn/gtyhinpnok.html

Py:   value = data or "默认值"
来源：http://hz.jinghuilouyu.cn/gtydioerah.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xuetiantiany.cn/gtcygqiklz.html


<!-- 参考信息 -->