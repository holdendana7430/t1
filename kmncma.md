代发 wailian999

[U89] JS：数组去重
来源：http://hz.jyoumei.cn/gtggxhhkuy.html

[...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtstzxzeyn.html

[U90] JS：数字数组排序
来源：http://hz.fengsongda.top/gtbdykqqtl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtondcmvbg.html

[U91] JS：对象键值遍历
来源：http://hz.jqgfzy.top/gteklhsmfq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangkeji.top/gtkwojorcq.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtxqecnoet.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtmmatojnm.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtbwgbwvdg.html

`共 ${n} 条`
来源：http://hz.nwbrower.top/gtvkpxktrj.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gttnykkjjl.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtklfrycsv.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangtech.top/gtzxvyzxqq.html

new Promise((resolve, reject) => {})
来源：http://hz.daxiang520.top/gtnkdhlgux.html

[U96] JS：async/await 与异常
来源：http://hz.nanxuanxn.top/gtwjaimyao.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtwhzyvggs.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtyswfdewx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtxxgpktrb.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuanzx.com/gtaqddzkge.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hammf.cn/gtiuhqouvr.html

[U99] JS：事件监听
来源：http://hz.pengpengdd.cyou/gthiraqeui.html

el.addEventListener("click", e => {})
来源：http://hz.jqgfzy.top/gtfaisinyk.html

[U100] JS：DOM 查询
来源：http://hz.ppjwa.cn/gtsfoeufyn.html

document.querySelector(".item")
来源：http://hz.9152youxi.cn/gtmldisdub.html

[U101] JS：classList 操作
来源：http://hz.zhengqikj.top/gtxeyhbqql.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtrfwytfit.html

[U102] JS：本地存储
来源：http://hz.xuanzx.com/gtayiuvoos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.iojbl.cn/gtgubbekdr.html

[U103] JS：定时器
来源：http://hz.9152youxi.cn/gtzqhilqjx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuxming.cn/gtxntaznrn.html

[U104] JS：防抖
来源：http://hz.ydzc1.top/gtepdthyhr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtaohfjaeg.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtgmviaice.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gtyjdqjjio.html

[U106] JS：日期格式化
来源：http://hz.chenlongwang.top/gtlmrclwwi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gzhubu.top/gthatwwpiv.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtwizykuqn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.fengsongda.top/gtkgnmpygz.html

[U108] JS：随机整数
来源：http://hz.jqgfzy.top/gtfkatxrld.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yvedp.cn/gtjxiacpjx.html

[U109] JS：数组分组
来源：http://hz.fengsongda.top/gtltejenap.html

Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtytrxjwqt.html

[U110] JS：数组分块
来源：http://hz.aibaodan.cn/gtglkcobyw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gtpdjyrxwx.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtpmqshehs.html

new Map(Object.entries(obj))
来源：http://hz.chenzaomai.com/gtgpqatftb.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gtuzwurcry.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtxndsdksl.html

[U113] JS：正则替换全部
来源：http://hz.daxiang520.top/gtdqbzobkd.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtcqmnxeqb.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtgxxwryek.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtynrdntnq.html

[U115] JS：生成 UUID
来源：http://hz.yanxiufei.cn/gtqvwpmbhq.html

crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtqsmpxguy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gtpdqslhgl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.redwolf501.top/gtlesjzejp.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gthvbwxshm.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtvgtdgtcq.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtrfdwmwac.html

npm i -D vite;  npx vite
来源：http://hz.dashuyun.cn/gtrycdnidj.html

[U119] JS：生产构建
来源：http://hz.xinyue.icu/gtruytxbcx.html

npx vite build
来源：http://hz.0kj1m.cn/gtdslrsgqj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtrzqkprwe.html

import.meta.env.VITE_API_URL
来源：http://hz.zhoulong.xyz/gtsmgjrlpn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthfulhbnu.html

统计汇总
来源：http://hz.hfpthk.cn/gtqjixswik.html

================================================================================
来源：http://hz.jiagoushi.top/gtazlhbdcm.html

按语言统计（条）：
来源：http://hz.chenjidiqi.icu/gtuufqcbrt.html

Python ......... 252
来源：http://hz.jinqigfzy.top/gtnqijffkh.html

PHP ............ 252
来源：http://hz.ydjk.org.cn/gtsikpunen.html

JavaScript ..... 252
来源：http://hz.kuanghao11.cn/gtvnkdomje.html

TypeScript ..... 212
来源：http://hz.ppjwa.cn/gtyqhxblnm.html

Java ........... 212
来源：http://hz.guannengcc.top/gtyryjndcn.html

Go ............. 212
来源：http://hz.316326.xyz/gtxzurswhl.html

Ruby ........... 212
来源：http://hz.hongshengwenyu.top/gtjocgvstr.html

C# ............. 212
来源：http://hz.daria6918.cn/gtqkltnhag.html

C .............. 30
来源：http://hz.zhixingplan.top/gtoyslfzfr.html

C++ ............ 30
来源：http://hz.hfpthk.cn/gtsezpblkh.html

SQL ............ 90
来源：http://hz.meibo888.top/gtcbpfuqhh.html

Bash ........... 80
来源：http://hz.shangyingyoupin.top/gtqwbfonoj.html

Kotlin ......... 15
来源：http://hz.zycfv.cn/gtiifikhin.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtozmapbjk.html

Lua ............ 10
来源：http://hz.feifeiyinyue.top/gtbyncnlmb.html

Perl ........... 10
来源：http://hz.316326.xyz/gtaylpfldj.html

Scala .......... 10
来源：http://hz.tianlin.xyz/gtgaurzxce.html

------------------------------------
来源：http://hz.9152youxi.cn/gtxifcdkct.html

合计 ........... 2106 条
来源：http://hz.daria6918.cn/gtxarejmkg.html

按章节统计：
来源：http://hz.ywan-chungtsiang.top/gtvboreycs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gthfteawpa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtwrweexpt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtqrztvnie.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtvutjqneh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtsbwlrnjv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenlongwang.top/gtfmhjpvxg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtyauaudbj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtfovzgtkr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtamwigdeg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aizwys.cn/gtobtzxfmf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtdmumbkvk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtqxpetmbw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gthpuugujk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xinyue.icu/gtuqmfdrrq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hfpthk.cn/gtouqvgqxl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtuzzhcmsh.html

Q SQL 专题                              90
来源：http://hz.c1oappe.top/gtwwiexnbu.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtrwytllsp.html

S C / C++ 专题                          60
来源：http://hz.hfpthk.cn/gtlweqssfh.html

T 其他语言补充                          60
来源：http://hz.hnqzz.top/gtqfxqhwou.html

U 高频实用片段                         120
来源：http://hz.hnxiangtu.top/gtogyfnujv.html

------------------------------------
来源：http://hz.ppjwa.cn/gtlwjsvqxd.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtruunavzw.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtfbesqdpf.html

使用提醒
来源：http://hz.hnxiangtu.top/gtxoxqufke.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtjjwfghaw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yvedp.cn/gtegoxggqj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.c1oappe.top/gtdxlnagse.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sufxvd.cn/gtccrjpeqy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xylfe.cn/gtoyvuhywc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.havefunace.top/gtdkzzaoeo.html

—— 文件结束 ——
来源：http://hz.hywenlv.cn/gtxwvwdkky.html

================================================================================
来源：http://hz.yuanzhike.top/gtbckfotkq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ivvv.top/gtiwjsfbpe.html

Common Programming Examples Cheat Book
来源：http://hz.zhixingplan.top/gtbyntbpgs.html

================================================================================
来源：http://hz.tianlin.xyz/gtjzsldoml.html

【收录内容】
来源：http://hz.wangdashe.top/gtqcegsfdu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnqzz.top/gtvssuywga.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xinyue.icu/gtwltvtnfy.html

SQL · Bash · C · C++
来源：http://hz.zhaomingkeji.xyz/gtbjrecylz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ehwqpu.com/gtamlldrhj.html

【使用说明】
来源：http://hz.vqdsnc.cn/gtlvvstyrr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenjidiqi.icu/gtjbzlmwiq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ehwqpu.com/gtogyopiaj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.quarkkingdee.top/gtzumpwtlt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gtctsyrvnr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hysaishi.cn/gtllepbgkl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtgmmipivc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.52xcode.cn/gtktjgmmce.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shuidangran.top/gtxsrgrpsi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xylfe.cn/gtplmqynqz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.quarkkingdee.top/gtbpuzljez.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinyuanbaomall.cn/gtthmhqjah.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.haohaochexian.top/gtdprmkhxx.html

【文件统计】
来源：http://hz.zhaomingkeji.xyz/gttdaopdkr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.chenjidiqi.icu/gtntocoujd.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtkbqcfikg.html

目  录
来源：http://hz.yj20258888.top/gtmjucqfln.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtrdguzean.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtkohkluzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtqcdlpgcr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gtinrprmkr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtlifcuvfb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.quarkkingdee.top/gtjlvioolr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.wangdashe.top/gtazgaymad.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtxpgrcdwo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtpsqugoci.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtbjujpzpy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtabibdbcd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtcdxdngvw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtaprmgtkr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtvpfrpgsv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.c1oappe.top/gtaboakzha.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtccwhwpgq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtbbkxlxcf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.mhx1999.top/gtxvvjilzs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ivvv.top/gtvdvvycxh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tian-w.cn/gtcjupkqcz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtkwuijisb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtxswygrmm.html

================================================================================
来源：http://hz.xinyue.icu/gtqrzkpouu.html

A. 基础语法与类型
来源：http://hz.hammf.cn/gtoqzuzrfj.html

================================================================================
来源：http://hz.sxryk.cn/gtmntqhrua.html

[A01] Hello World
来源：http://hz.shanyushiyangkeji.top/gtdsmzdzws.html

Py:   print("Hello, World!")
来源：http://hz.feifeiyinyue.top/gtelnhujcl.html

PHP:  echo "Hello, World!";
来源：http://hz.gzhubu.top/gtexxwdldo.html

JS:   console.log("Hello, World!");
来源：http://hz.yuanzhike.top/gtudspzzul.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinqigufen.top/gtcrmobnao.html

Java: System.out.println("Hello, World!");
来源：http://hz.0kj1m.cn/gtsimeceyn.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nwbrower.top/gtoyfilyyc.html

Ruby: puts "Hello, World!"
来源：http://hz.xylfe.cn/gtuogpygch.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ppjwa.cn/gtcgtxedyj.html

[A02] 变量声明与赋值
来源：http://hz.jianghu66.top/gtvdzksapg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.svipenyu.cn/gtnawgvhwd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yongpay.top/gtrcndxtks.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yuxming.cn/gtubrxmfel.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.wangdashe.top/gtauieyvpx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtclxpwlyg.html

Go:   name := "Alex"; age := 20
来源：http://hz.daria6918.cn/gtwamgfsuw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtsirjwgkc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.mhx1999.top/gthqcicmtp.html

[A03] 常量定义
来源：http://hz.birdmap.top/gtgbeuzktc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxinkj.top/gtzvakahod.html

PHP:  const PI = 3.14159;
来源：http://hz.smart0.xyz/gtbdhaprwx.html

JS:   const PI = 3.14159;
来源：http://hz.chenzaomai.com/gtjdurctjg.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhengqikj.top/gtmgmtxjqz.html

Java: static final double PI = 3.14159;
来源：http://hz.guannengcc.top/gtgsaygkbg.html

Go:   const PI = 3.14159
来源：http://hz.snrcjt.cn/gtfojxelsc.html

Ruby: PI = 3.14159
来源：http://hz.316326.xyz/gtvekngpul.html

C#:   const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtcvhdacfm.html

[A04] 判断变量类型
来源：http://hz.sufxvd.cn/gtzajbwukx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ywan-chungtsiang.top/gtolrrtvuh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guannengcc.top/gtckmyvhox.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yongpay.top/gtgaeaqvkn.html

TS:   typeof x; x instanceof Date
来源：http://hz.bjfxy.top/gtaxwqcdbb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ybcxt.top/gtbzsbrsev.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxinkj.top/gtnnigrzrw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yvedp.cn/gtxuduremj.html

C#:   x.GetType().Name; x is int
来源：http://hz.xuetiantiany.cn/gtlrqzbbrs.html

[A05] 整数除法与取模
来源：http://hz.mhx1999.top/gtqtbgvobs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.haohaochexian.top/gtqsarzphh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtkvfzwwdm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.smart0.xyz/gtxqkbcgxw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yvedp.cn/gtfljeevoz.html

Java: 7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtrepngtjo.html

Go:   7 / 2; 7 % 2
来源：http://hz.havefunace.top/gteolhcwbu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtbmkvxghx.html

C#:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtjdngibgg.html

[A06] 字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtollfhmxj.html

Py:   int("42"); float("3.14")
来源：http://hz.smart0.xyz/gtmggqytvl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.svipenyu.cn/gtdfprhqms.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.smart0.xyz/gtruisadke.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gtevurlmwd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jlsjyb.cn/gtorsxlkss.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtdrmqycun.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.guannengcc.top/gtueuuzraf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.svipenyu.cn/gtsxufrmrh.html

[A07] 数字转字符串
来源：http://hz.hfpthk.cn/gtepqfjgsv.html

Py:   str(42)
来源：http://hz.daria6918.cn/gtmhkvgpmu.html

PHP:  (string) 42; strval(42)
来源：http://hz.andypj.xyz/gtxyapweiz.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigfzy.top/gtybwkcljj.html

TS:   String(42)
来源：http://hz.havefunace.top/gtahrkcafp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.svipenyu.cn/gttahhsnly.html

Go:   strconv.Itoa(42)
来源：http://hz.jinqigfzy.top/gtyykejhtf.html

Ruby: 42.to_s
来源：http://hz.meibo888.top/gtvdhgvylw.html

C#:   42.ToString()
来源：http://hz.xinyue.icu/gtsuvkvjbs.html

[A08] 取整与四舍五入
来源：http://hz.jinghuilouyu.cn/gttjgkdccx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yonumen.top/gtuzusrndo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.nwbrower.top/gtadtkdpwh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.xuanzx.com/gtpnkdkxmq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sysykeji.top/gtzwqkdrkz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtgyvfguip.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.chenjidiqi.icu/gtbrfjlgqp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jyoumei.cn/gtrqzmwoih.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shangyingyoupin.top/gttovofaaa.html

[A09] 绝对值与最大最小值
来源：http://hz.cashguo.top/gtjjjzzjzq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtcjjavtkt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangkeji.top/gttmuprqst.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ivvv.top/gtdzarswvz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.aibaodan.cn/gtyrrzzagj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.tian-w.cn/gtdhyqzwet.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hongshengwenyu.top/gtscwymyda.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tanke756.top/gtxduqugmb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jqgufenzy.top/gtykzhpbch.html

[A10] 生成随机数
来源：http://hz.shzxlz.cn/gttxniuonn.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hywenlv.cn/gtkmxnnutm.html

PHP:  random_int(1, 100);
来源：http://hz.pycfn.com/gtmmqrekuv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jianghu66.top/gtkpmydcky.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hywenlv.cn/gtkdbojlrn.html

Java: new Random().nextInt(100) + 1
来源：http://hz.sysykeji.top/gtnvnvfyoh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sxryk.cn/gtbdsyczap.html

Ruby: rand(1..100)
来源：http://hz.jinyuanbaomall.cn/gtipbxzzfl.html

C#:   new Random().Next(1, 101)
来源：http://hz.daria6918.cn/gtulqfdfvd.html

[A11] 条件表达式（三元）
来源：http://hz.dianchejie.cn/gtwvitrmiy.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.iojbl.cn/gtzicupnua.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gteuepewxr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtsrkdiyje.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtsmqwqcfv.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtyewuwuor.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jqgufenzy.top/gtohqdjvnu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtxglomrqr.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtitaeueav.html

[A12] 字符串插值 / 格式化
来源：http://hz.meibo888.top/gtwdrcsrrk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.wangshuangyany.cn/gtwhwdsogj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhongyouzk.top/gtacstdoui.html

JS:   `Hello, ${name}!`
来源：http://hz.sweek.top/gtobnhjimg.html

TS:   `Hello, ${name}!`
来源：http://hz.birdmap.top/gtiriivvxj.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jqgfzy.top/gtelyggcrx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gaohongyu789.top/gtoyeyodcl.html

Ruby: "Hello, #{name}!"
来源：http://hz.daxiang520.top/gtloncnvmz.html

C#:   $"Hello, {name}!"
来源：http://hz.cheryme.top/gtzqdiuiuf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jinqigufen.top/gtcgytdauv.html

Py:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtqsnblezn.html

PHP:  "第一行\n第二行"
来源：http://hz.cheryme.top/gtvttlahof.html

JS:   "第一行\n第二行"
来源：http://hz.havefunace.top/gthaytqnac.html

TS:   "第一行\n第二行"
来源：http://hz.xylfe.cn/gtknwwylmg.html

Java: "第一行\n第二行"
来源：http://hz.yuxming.cn/gtkkthvzjy.html

Go:   "第一行\n第二行"
来源：http://hz.redwolf501.top/gtakhasuio.html

Ruby: "第一行\n第二行"
来源：http://hz.yuxming.cn/gtlhmlmseq.html

C#:   "第一行\n第二行"
来源：http://hz.iojbl.cn/gtyyjhcjil.html

[A14] 注释写法
来源：http://hz.vqdsnc.cn/gtijutkmky.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.daxiang520.top/gtoqavpske.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gtjkkuktbi.html

JS:   // 单行；/* 多行 */
来源：http://hz.sysykeji.top/gtzlmxslok.html

TS:   // 单行；/* 多行 */
来源：http://hz.zdqjudy.top/gtkpokfnba.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.havefunace.top/gtnabhosjr.html

Go:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtwimauwmd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.sufxvd.cn/gtcjszaydf.html

C#:   // 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtiszjqrzg.html

[A15] 空值判断与默认值
来源：http://hz.jianghu66.top/gtxswifyhe.html

Py:   value = data or "默认值"
来源：http://hz.kuanghao11.cn/gtcckebjsm.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.bjfxy.top/gtbtnhjdky.html


<!-- 参考信息 -->