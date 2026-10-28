代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.cdnleiting.top/gthqzugwxh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258888.top/gtniwbhebm.html

[U92] JS：深拷贝
来源：http://hz.xinyue.icu/gtqigrxklr.html

structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtysntdcjz.html

[U93] JS：模板字符串
来源：http://hz.c1oappe.top/gtrwppazax.html

`共 ${n} 条`
来源：http://hz.jianghu66.top/gtakdwjyhj.html

[U94] JS：箭头函数
来源：http://hz.xziqi.cn/gthipsmmfr.html

const double = x => x * 2;
来源：http://hz.wangdashe.top/gtlmovnamz.html

[U95] JS：Promise 包装
来源：http://hz.zycfv.cn/gtuiccdutu.html

new Promise((resolve, reject) => {})
来源：http://hz.cqqwz.cn/gtafwlxcpd.html

[U96] JS：async/await 与异常
来源：http://hz.tianlin.xyz/gtzqvpfpsi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gthpjsfcrh.html

[U97] JS：并发请求
来源：http://hz.bjfxy.top/gtoiyzwpdf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtcofxoles.html

[U98] JS：fetch 带 JSON
来源：http://hz.bjfxy.top/gtpfjflgqw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj20258888.top/gtgdggbkuw.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gtjvvkzprn.html

el.addEventListener("click", e => {})
来源：http://hz.dashuyun.cn/gtvfvvdysv.html

[U100] JS：DOM 查询
来源：http://hz.hammf.cn/gtbchewhtd.html

document.querySelector(".item")
来源：http://hz.snrcjt.cn/gtsqhbeyqw.html

[U101] JS：classList 操作
来源：http://hz.c1oappe.top/gtafdmvgjv.html

el.classList.toggle("active")
来源：http://hz.aibaodan.cn/gtpfhqzxls.html

[U102] JS：本地存储
来源：http://hz.jyoumei.cn/gtasuhfbax.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigfzy.top/gtvfjjimbs.html

[U103] JS：定时器
来源：http://hz.jinghuilouyu.cn/gtnhzhkywr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yvedp.cn/gtpkngrrxk.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gtliegigvc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtqhrrrbyf.html

[U105] JS：节流
来源：http://hz.svipenyu.cn/gthbkscofd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zdqjudy.top/gtvbaacdcw.html

[U106] JS：日期格式化
来源：http://hz.shanyushiyangtech.top/gtzzxkquok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tanke756.top/gtzeamzwzw.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gthmrzuvlv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yueranfly.top/gtimpxsmjj.html

[U108] JS：随机整数
来源：http://hz.ehwqpu.com/gtiokwlhlt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zycfv.cn/gtnoudsyhu.html

[U109] JS：数组分组
来源：http://hz.zhixingplan.top/gtqcsvotam.html

Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtrkutamum.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtxoimadhv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guannengcc.top/gtyuevevlc.html

[U111] JS：对象转 Map
来源：http://hz.sufxvd.cn/gtwjrqynwy.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gtkmtjuyuo.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtmjaefxgw.html

"7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtpvvnuzdg.html

[U113] JS：正则替换全部
来源：http://hz.kuanghao11.cn/gtaftzxdij.html

s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtmnrdnxtf.html

[U114] JS：JSON 深比较
来源：http://hz.sufxvd.cn/gtribhozux.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtrkabzapy.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtziamrhyn.html

crypto.randomUUID()
来源：http://hz.yongpay.top/gtcocacovh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shzxlz.cn/gtquiqgcuf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daria6918.cn/gtlieqfojy.html

[U117] JS：单元测试
来源：http://hz.sysykeji.top/gtmlwukelb.html

npm i -D vitest;  npx vitest
来源：http://hz.mhx1999.top/gtbmkpfxyi.html

[U118] JS：开发服务器
来源：http://hz.aibaodan.cn/gtoewrmbqj.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gtsdykcvye.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtzvjmtnhp.html

npx vite build
来源：http://hz.daria6918.cn/gtikpuoleu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hywenlv.cn/gtsrxjrdvq.html

import.meta.env.VITE_API_URL
来源：http://hz.tianlin.xyz/gtkzhbkoay.html

================================================================================
来源：http://hz.pycfn.com/gtwxjjexwi.html

统计汇总
来源：http://hz.316326.xyz/gtmgsjzvxy.html

================================================================================
来源：http://hz.fzhhl.top/gtjlajjoln.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtdcafcjaz.html

Python ......... 252
来源：http://hz.aibaodan.cn/gtzgqumjer.html

PHP ............ 252
来源：http://hz.xuanzx.com/gtwueeorja.html

JavaScript ..... 252
来源：http://hz.gaohongyu789.top/gtbfeusznl.html

TypeScript ..... 212
来源：http://hz.xinyue.icu/gtdeecensc.html

Java ........... 212
来源：http://hz.yueranfly.top/gtlyuowmfl.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gtydtaantt.html

Ruby ........... 212
来源：http://hz.zhixingplan.top/gtydmcubra.html

C# ............. 212
来源：http://hz.xuetiantiany.cn/gtpwyoqezj.html

C .............. 30
来源：http://hz.gogol.net.cn/gtswxtgyms.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtpvorugsm.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtpalkrvzn.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gtanwepqnq.html

Kotlin ......... 15
来源：http://hz.nanxinkj.top/gttjrthrgu.html

Swift .......... 15
来源：http://hz.snrcjt.cn/gtfwfgozeh.html

Lua ............ 10
来源：http://hz.xylfe.cn/gtxspaisey.html

Perl ........... 10
来源：http://hz.birdmap.top/gttacpiegs.html

Scala .......... 10
来源：http://hz.c1oappe.top/gtjhfpwxut.html

------------------------------------
来源：http://hz.zycfv.cn/gtakqgasdc.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtzgxsalsm.html

按章节统计：
来源：http://hz.nanxinkj.top/gteysmxhmt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtzxldtldf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtifuvdcfz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtykjdmvkm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gthepiypcz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tian-w.cn/gtodztdgnt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gthntelhej.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtiidlbrhi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gtoctjevax.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtcgsuecmu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtymfijkph.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtotabipwi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtqtwvcmmq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gthvbesrjv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtikjhtvbt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gtoaxtzcuc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtqckvmrke.html

Q SQL 专题                              90
来源：http://hz.jiagoushi.top/gtqqtpthib.html

R Bash 专题                             80
来源：http://hz.nanxuanxn.top/gtqqebndnm.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtnsnebxkl.html

T 其他语言补充                          60
来源：http://hz.ybcxt.top/gtfydvpytl.html

U 高频实用片段                         120
来源：http://hz.haohaochexian.top/gtpcrlznyj.html

------------------------------------
来源：http://hz.guowangkeji.top/gtpjohjzdp.html

合计                                  2106 条
来源：http://hz.ydzc1.top/gtomribumc.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtepcyghka.html

使用提醒
来源：http://hz.ybcxt.top/gtdbjizoij.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtooozczgx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinyuanbaomall.cn/gtayxnkvaw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.meibo888.top/gtmayqdpjv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gtfukbkdfb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.feifeiyinyue.top/gtdrsyudfr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xinyue.icu/gtbfkhvajq.html

—— 文件结束 ——
来源：http://hz.chenzaomai.com/gtacptqfmt.html

================================================================================
来源：http://hz.jyoumei.cn/gtjsbbkidw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenjidiqi.icu/gtlxhsckrh.html

Common Programming Examples Cheat Book
来源：http://hz.ehwqpu.com/gtiemabmya.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqjohvdwg.html

【收录内容】
来源：http://hz.svipenyu.cn/gtavafqurm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jianghu66.top/gtvmnsnvnc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhijiandao.cn/gtfrxvyjhg.html

SQL · Bash · C · C++
来源：http://hz.shangyingyoupin.top/gterxrcwdf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yuanzhike.top/gtwxnupeoq.html

【使用说明】
来源：http://hz.jinyuanbaomall.cn/gtbdnazedk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangtech.top/gtinaruhpe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.bjfxy.top/gthqxlslji.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.quarkkingdee.top/gtsuqmujel.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.daxiang520.top/gtjmypazru.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtbadsniiz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhixingplan.top/gtauxpzopk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.havefunace.top/gtfllulniy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.redwolf501.top/gttoecyrza.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hammf.cn/gtlryxbjhc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gotoacloud.top/gtldrjhhva.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ppjwa.cn/gtphxlvovd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nanxinkj.top/gtxmddipgw.html

【文件统计】
来源：http://hz.316326.xyz/gtxbvwpcmz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.316326.xyz/gteqhxmrgf.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gttpzjrtwu.html

目  录
来源：http://hz.shanyushiyangtech.top/gtxqcnoalq.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtbbbnuufy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xuetiantiany.cn/gtjxetsjnk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtqqfdmbzs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hnxiangtu.top/gtvqtgmxbt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shuidangran.top/gtmzrporsp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.quarkkingdee.top/gtzhdzqbtb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.dashuyun.cn/gttrngiijc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtafbrghtb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtcmkqenap.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gtjcgnrobd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtpvltrvwq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtgomrjnnw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtfnnefmgd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtlmknpsck.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.bjfxy.top/gtgqdvaidx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sweek.top/gtqirrstgw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtzrhxqlin.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuetiantiany.cn/gtkqnvmngs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gthmkkjfyj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shuidangran.top/gtuzuiwacg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtkswkomaa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtdplbmepi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtmnnuaaum.html

A. 基础语法与类型
来源：http://hz.sxryk.cn/gtelhwsvoa.html

================================================================================
来源：http://hz.haohaochexian.top/gtclkvyfmz.html

[A01] Hello World
来源：http://hz.wangshuangyany.cn/gtfbzbneix.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtvnlcfeln.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigfzy.top/gttywbibow.html

JS:   console.log("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtthroouvn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sysykeji.top/gtmkwirmjz.html

Java: System.out.println("Hello, World!");
来源：http://hz.birdmap.top/gtspmbquif.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.dianchejie.cn/gtuaqajnnm.html

Ruby: puts "Hello, World!"
来源：http://hz.redwolf501.top/gtlbytgagu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.guowangkeji.top/gtokztwkdv.html

[A02] 变量声明与赋值
来源：http://hz.jinqigufen.top/gtadsjqxep.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hongshengwenyu.top/gtmwsewyyi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yj202588.top/gtjwreeqyr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuetiantiany.cn/gtinqpzrve.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ivvv.top/gtdxzxlcwc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnxiangtu.top/gtftdpciid.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gtywexlgdf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.haohaochexian.top/gtzuwidtkp.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtugsfbxao.html

[A03] 常量定义
来源：http://hz.yj20258888.top/gtnzyuztkb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hywenlv.cn/gtfjdxqjmo.html

PHP:  const PI = 3.14159;
来源：http://hz.9152youxi.cn/gtjvjutsfd.html

JS:   const PI = 3.14159;
来源：http://hz.yvedp.cn/gtgrenxiud.html

TS:   const PI: number = 3.14159;
来源：http://hz.gogol.net.cn/gthxhmirts.html

Java: static final double PI = 3.14159;
来源：http://hz.meibo888.top/gtgpxdzeis.html

Go:   const PI = 3.14159
来源：http://hz.jinyuanbaomall.cn/gtvkngjsft.html

Ruby: PI = 3.14159
来源：http://hz.zhijiandao.cn/gteqyaqzsr.html

C#:   const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtgdmofdeq.html

[A04] 判断变量类型
来源：http://hz.ppjwa.cn/gtqvtsppmu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.dashuyun.cn/gteeutcdrn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zycfv.cn/gtmdbxynja.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cheryme.top/gtxlhlxbbj.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtapyuzvqv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.mhx1999.top/gtenqkmdvp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.kuanghao11.cn/gtefioqxhe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hammf.cn/gtgucedgqv.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgufenzy.top/gtqfywamka.html

[A05] 整数除法与取模
来源：http://hz.pycfn.com/gtuxfuwbgl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tian-w.cn/gtmxpjnubf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.mhx1999.top/gtumpqbpky.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gthtidkysj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.chenzaomai.com/gtffffison.html

Java: 7 / 2; 7 % 2
来源：http://hz.iojbl.cn/gtedsizmot.html

Go:   7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtpkucwqcv.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gtglocrvrx.html

C#:   7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gtgoyxbrqx.html

[A06] 字符串转数字
来源：http://hz.zhongyouzk.top/gtlbpqylbk.html

Py:   int("42"); float("3.14")
来源：http://hz.yueranfly.top/gtpfzzkxeo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gzhubu.top/gtfksjbqrf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ehwqpu.com/gtktcftjjt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.fzhhl.top/gtruzagazl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.316326.xyz/gtalwptckj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yangfankeji.com/gtttlqhwwv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ydzc1.top/gtvmjdlgtv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jianghu66.top/gttprcighk.html

[A07] 数字转字符串
来源：http://hz.birdmap.top/gtgozraind.html

Py:   str(42)
来源：http://hz.9152youxi.cn/gtpfeemuwi.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhaomingkeji.xyz/gtsnnxhvcj.html

JS:   String(42); (42).toString()
来源：http://hz.daxiang520.top/gtrhnyoxyx.html

TS:   String(42)
来源：http://hz.sysykeji.top/gtvxdifvsm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xuetiantiany.cn/gtzffvvibm.html

Go:   strconv.Itoa(42)
来源：http://hz.mhx1999.top/gtevbnnvfm.html

Ruby: 42.to_s
来源：http://hz.jlsjyb.cn/gtqfvspmmt.html

C#:   42.ToString()
来源：http://hz.redwolf501.top/gtnuhabvgw.html

[A08] 取整与四舍五入
来源：http://hz.hammf.cn/gtmobhlelc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hysaishi.cn/gtgrotmffc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jyoumei.cn/gthnlncqsy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ybcxt.top/gtavlwcmcf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jqgufenzy.top/gthvqugoom.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.aizwys.cn/gtgbqiredt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.c1oappe.top/gttlwroxez.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.smart0.xyz/gtuwqwrogp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xuanzx.com/gtswzesaax.html

[A09] 绝对值与最大最小值
来源：http://hz.hywenlv.cn/gtwpxlfsfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.pycfn.com/gtaclptbco.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jiagoushi.top/gttaifrjdo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.aibaodan.cn/gtcnhmujif.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtpccjszrk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.316326.xyz/gtulnumluf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.redwolf501.top/gtueqxnrfg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhijiandao.cn/gtpvricodk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yongpay.top/gtfkrqbosw.html

[A10] 生成随机数
来源：http://hz.guannengcc.top/gthspjtgfv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xuetiantiany.cn/gtkyggfhia.html

PHP:  random_int(1, 100);
来源：http://hz.zhoulong.xyz/gtnpexcaxl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yj20258888.top/gtjskdzhvb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigfzy.top/gtosvyjqyo.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hywenlv.cn/gtvvoitrlb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhiwuduotai.top/gtpfcxdkwz.html

Ruby: rand(1..100)
来源：http://hz.yj202588.top/gtmhdmogbc.html

C#:   new Random().Next(1, 101)
来源：http://hz.yvedp.cn/gtndjykojq.html

[A11] 条件表达式（三元）
来源：http://hz.zhixingplan.top/gtqllfhqju.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.haohaochexian.top/gtjhbiojsq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtfdvzfdak.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ivvv.top/gttgalgzza.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtziotemob.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtwzsulqkf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.iojbl.cn/gtqzuaswsj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.gotoacloud.top/gtgigqzxcg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gtueyikvvw.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhoulong.xyz/gtbqburlpy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.sweek.top/gtaojroqew.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ppjwa.cn/gtbnplzlzy.html

JS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangtech.top/gtjldtkbke.html

TS:   `Hello, ${name}!`
来源：http://hz.dianchejie.cn/gthagqquux.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hammf.cn/gtmkzdfseb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.chenzaomai.com/gtqpgnhcjt.html

Ruby: "Hello, #{name}!"
来源：http://hz.xinyue.icu/gtfsydknwl.html

C#:   $"Hello, {name}!"
来源：http://hz.smart0.xyz/gtzelwpnns.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ydjk.org.cn/gtsnelvojc.html

Py:   "第一行\n第二行"
来源：http://hz.yongpay.top/gtqxntcjio.html

PHP:  "第一行\n第二行"
来源：http://hz.ydzc1.top/gtkjqwbhoq.html

JS:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtidxajvnn.html

TS:   "第一行\n第二行"
来源：http://hz.gogol.net.cn/gtnehkrfyv.html

Java: "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtesnenzua.html

Go:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtyoncersc.html

Ruby: "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtjdkosvyv.html

C#:   "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtwiejbscz.html

[A14] 注释写法
来源：http://hz.yongpay.top/gtxbkrfwco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.guowangkeji.top/gtmipycgan.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtjyyhwngj.html

JS:   // 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtyppphcpb.html

TS:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtxdpnteru.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhengqikj.top/gtsrfxwypt.html

Go:   // 单行；/* 多行 */
来源：http://hz.jinyuanbaomall.cn/gtycwyqcdi.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.cheryme.top/gtsuclbriu.html

C#:   // 单行；/* 多行 */
来源：http://hz.jqgfzy.top/gtrzlyahtv.html

[A15] 空值判断与默认值
来源：http://hz.yueranfly.top/gtzdjcezrj.html

Py:   value = data or "默认值"
来源：http://hz.xingfuxueyuan.xyz/gtjnomnwlf.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guannengcc.top/gtgcbnhfec.html

JS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtqukycuqm.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtvbkzpbqv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nwbrower.top/gtvpbeowiy.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.fzhhl.top/gtbcokqalh.html


<!-- 参考信息 -->