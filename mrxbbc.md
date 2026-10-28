代发 wailian999

[U87] JS：解构默认值
来源：http://hz.daria6918.cn/gtkefukvol.html

const { a = 1, b = 2 } = obj;
来源：http://hz.feifeiyinyue.top/gtqiujxsem.html

[U88] JS：对象展开合并
来源：http://hz.jqgfzy.top/gtvmnygpmh.html

{ ...a, ...b }
来源：http://hz.jinghuilouyu.cn/gtzppecjta.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtaepefpxz.html

[...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtfiscsxbk.html

[U90] JS：数字数组排序
来源：http://hz.hfpthk.cn/gtfazuqoca.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gthuddgvgi.html

[U91] JS：对象键值遍历
来源：http://hz.c1oappe.top/gtxzzqlljn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangtech.top/gtdqcelggd.html

[U92] JS：深拷贝
来源：http://hz.jinyuanbaomall.cn/gtboksuozd.html

structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtyjntfpgv.html

[U93] JS：模板字符串
来源：http://hz.xziqi.cn/gtgrleaoey.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtikvyejol.html

[U94] JS：箭头函数
来源：http://hz.zycfv.cn/gtzcdrpplm.html

const double = x => x * 2;
来源：http://hz.zdqjudy.top/gtkxxgoasn.html

[U95] JS：Promise 包装
来源：http://hz.shangyingyoupin.top/gtybvxggkd.html

new Promise((resolve, reject) => {})
来源：http://hz.gzhubu.top/gtadqbbkpj.html

[U96] JS：async/await 与异常
来源：http://hz.jinyuanbaomall.cn/gtptralqgp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtgvhsesbs.html

[U97] JS：并发请求
来源：http://hz.pengpengdd.cyou/gtfpfbidpr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtzhsugzdu.html

[U98] JS：fetch 带 JSON
来源：http://hz.aizwys.cn/gtgkrnlnlr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxuanxn.top/gtdqyktkep.html

[U99] JS：事件监听
来源：http://hz.yongpay.top/gtzdpyzstd.html

el.addEventListener("click", e => {})
来源：http://hz.52xcode.cn/gtbjqnqgke.html

[U100] JS：DOM 查询
来源：http://hz.snrcjt.cn/gtgqfxbota.html

document.querySelector(".item")
来源：http://hz.cheryme.top/gtviezoyte.html

[U101] JS：classList 操作
来源：http://hz.hammf.cn/gtaftfwdtf.html

el.classList.toggle("active")
来源：http://hz.nanxuanxn.top/gtwblimdvz.html

[U102] JS：本地存储
来源：http://hz.shzxlz.cn/gtexkjgxfx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinghuilouyu.cn/gtbsuzzuga.html

[U103] JS：定时器
来源：http://hz.wangshuangyany.cn/gtsxkubgyj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ybcxt.top/gtregxewax.html

[U104] JS：防抖
来源：http://hz.nwbrower.top/gtlelvzidz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gthmshapnd.html

[U105] JS：节流
来源：http://hz.cucudq.cn/gtbulvcyep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigufen.top/gtyuccvbqu.html

[U106] JS：日期格式化
来源：http://hz.jinghuilouyu.cn/gtmnsqwjgs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenjidiqi.icu/gtscwgsuxi.html

[U107] JS：数字千分位
来源：http://hz.pengpengdd.cyou/gtdprjgxkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.iojbl.cn/gtllayhnfx.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangtech.top/gtdwntegyx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gtkjdbyulv.html

[U109] JS：数组分组
来源：http://hz.daxiang520.top/gtmzfgdalp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtkffmjyij.html

[U110] JS：数组分块
来源：http://hz.aizwys.cn/gtsbkuyjyn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.mhx1999.top/gtlsovvzme.html

[U111] JS：对象转 Map
来源：http://hz.haohaochexian.top/gtpnzslisz.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtvdepwxgd.html

[U112] JS：字符串补位
来源：http://hz.sufxvd.cn/gtvbgtecsb.html

"7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtsgekgczm.html

[U113] JS：正则替换全部
来源：http://hz.tianlin.xyz/gtmyjwheup.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gteoedoxok.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtohdigzmg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtdpgeesgg.html

[U115] JS：生成 UUID
来源：http://hz.0kj1m.cn/gteqqmmrvv.html

crypto.randomUUID()
来源：http://hz.smart0.xyz/gtsobnsmkx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hysaishi.cn/gttnkfzzce.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtbisipfdv.html

[U117] JS：单元测试
来源：http://hz.hnqzz.top/gtbxqayuel.html

npm i -D vitest;  npx vitest
来源：http://hz.pycfn.com/gtbrikkcmb.html

[U118] JS：开发服务器
来源：http://hz.fengsongda.top/gtzfmgogev.html

npm i -D vite;  npx vite
来源：http://hz.tian-w.cn/gtyddpdlrr.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gtqpkemcsq.html

npx vite build
来源：http://hz.xylfe.cn/gtoswtwjpf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daria6918.cn/gtffhxcfpf.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtcqypuqkk.html

================================================================================
来源：http://hz.hywenlv.cn/gtzjqaomih.html

统计汇总
来源：http://hz.daxiang520.top/gtmrlpcdly.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthozmovjp.html

按语言统计（条）：
来源：http://hz.jqgufenzy.top/gtjgllvnvv.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtbgbqvjfv.html

PHP ............ 252
来源：http://hz.cucudq.cn/gtbmsthxgz.html

JavaScript ..... 252
来源：http://hz.jinghuilouyu.cn/gttqvnwopf.html

TypeScript ..... 212
来源：http://hz.jinqigufen.top/gtrhpgorgq.html

Java ........... 212
来源：http://hz.zdqjudy.top/gtwpxigfbk.html

Go ............. 212
来源：http://hz.zhixingplan.top/gtbbkfpfdq.html

Ruby ........... 212
来源：http://hz.guowangkeji.top/gtwfrrgkcp.html

C# ............. 212
来源：http://hz.c1oappe.top/gtygchpsxq.html

C .............. 30
来源：http://hz.gaohongyu789.top/gteeocssog.html

C++ ............ 30
来源：http://hz.chenzaomai.com/gtodzjagie.html

SQL ............ 90
来源：http://hz.ydzc1.top/gtqffqabzk.html

Bash ........... 80
来源：http://hz.yuxming.cn/gtipagbsln.html

Kotlin ......... 15
来源：http://hz.svipenyu.cn/gtskpmfpzu.html

Swift .......... 15
来源：http://hz.cdnleiting.top/gtbqoofmua.html

Lua ............ 10
来源：http://hz.yuxming.cn/gtddllaluw.html

Perl ........... 10
来源：http://hz.yongpay.top/gtbmauiwmo.html

Scala .......... 10
来源：http://hz.chenlongwang.top/gtaixaapjv.html

------------------------------------
来源：http://hz.yj202588.top/gtbdedbbpu.html

合计 ........... 2106 条
来源：http://hz.xziqi.cn/gtebogemda.html

按章节统计：
来源：http://hz.xziqi.cn/gtjulnegvv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtbsjupxij.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtxiozqyhv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtwhamredg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtkprcnmex.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.gogol.net.cn/gtmaaixgcs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtkbbcblvo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtasvxqebb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gthxkgmlya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtjoqkfriy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtappnurdi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258888.top/gtxbutcwor.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtqnqqkdty.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtotquxwlk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ydjk.org.cn/gtotrtsysw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.feifeiyinyue.top/gtvrxxufpi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtemzxqpuz.html

Q SQL 专题                              90
来源：http://hz.xylfe.cn/gtjwwlshhd.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtydiqxrcq.html

S C / C++ 专题                          60
来源：http://hz.smart0.xyz/gtiqfgjapz.html

T 其他语言补充                          60
来源：http://hz.yj20258888.top/gtayczdupn.html

U 高频实用片段                         120
来源：http://hz.hongshengwenyu.top/gtdhnvltoy.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtsmkruvby.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtcqlgygot.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtxrxiwzns.html

使用提醒
来源：http://hz.daxiang520.top/gtvlprkixa.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtininzezb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hysaishi.cn/gtjcogkiqu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ivvv.top/gtaworzajy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhiwuduotai.top/gtwhpswwik.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gaohongyu789.top/gtmxdutwhd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sufxvd.cn/gtqsyhhiyu.html

—— 文件结束 ——
来源：http://hz.ehwqpu.com/gtwwsrhigi.html

================================================================================
来源：http://hz.ydzc1.top/gtokpghkns.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hnqzz.top/gtycmnszpz.html

Common Programming Examples Cheat Book
来源：http://hz.gotoacloud.top/gtzzpvlykh.html

================================================================================
来源：http://hz.gotoacloud.top/gtxmstnllp.html

【收录内容】
来源：http://hz.jlsjyb.cn/gtmevvfhxm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daria6918.cn/gtipllqujr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fengsongda.top/gtpbrlflbz.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtilgkvndi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sxryk.cn/gtlqpykurj.html

【使用说明】
来源：http://hz.nanxuanxn.top/gtjrjudwag.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ydzc1.top/gttaxyvdjy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ehwqpu.com/gtcnvjsuin.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.guannengcc.top/gtophedjbh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gogol.net.cn/gtrpfhnxtf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xinyue.icu/gthlxemacl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.bjfxy.top/gtkgvevagd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.nanxinkj.top/gtfidpoxev.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shanyushiyangkeji.top/gteebjukmx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yueranfly.top/gtzuphgkte.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.snrcjt.cn/gtjhepniwy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.cashguo.top/gtkezxpzgh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtwhelvwjx.html

【文件统计】
来源：http://hz.jlsjyb.cn/gtvxmjusex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shuidangran.top/gtpevlxssy.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtpwnejosu.html

目  录
来源：http://hz.shzxlz.cn/gtrdwclupl.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtmhvqvyvk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtkcwdefsd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gthldytqms.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtvivvcczx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gthiasdxpi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.kuanghao11.cn/gteznwvdyt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinqigfzy.top/gtnxcapamv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtqcbbyoof.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jlsjyb.cn/gtpkmesurr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtrolqingw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.chenzaomai.com/gtnfocqzxm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtvucwikws.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtuqwovxhb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gttpobwthf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jyoumei.cn/gtzjgnyhnv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhijiandao.cn/gtzzgirrgo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gttzcomsfi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtenwuikfk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sweek.top/gtebsgnyps.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tanke756.top/gthyyminbv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtuvxzytrz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtnvcsvdhw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjpbmqjvb.html

A. 基础语法与类型
来源：http://hz.jqgufenzy.top/gtjyryepgq.html

================================================================================
来源：http://hz.wangdashe.top/gtzgyzonbu.html

[A01] Hello World
来源：http://hz.316326.xyz/gtgirknetc.html

Py:   print("Hello, World!")
来源：http://hz.meibo888.top/gtglarrvvy.html

PHP:  echo "Hello, World!";
来源：http://hz.yuxming.cn/gtkmtvxdio.html

JS:   console.log("Hello, World!");
来源：http://hz.ybcxt.top/gtxmbpgkhv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.snrcjt.cn/gtgxfifdyw.html

Java: System.out.println("Hello, World!");
来源：http://hz.yvedp.cn/gtxwxtaivd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtweqslmzq.html

Ruby: puts "Hello, World!"
来源：http://hz.shuidangran.top/gtnmnlensj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.c1oappe.top/gtazfbpdpl.html

[A02] 变量声明与赋值
来源：http://hz.shanyushiyangtech.top/gtobwudeuw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.daxiang520.top/gtapdpkfiy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ywan-chungtsiang.top/gtxtriywbv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhengqikj.top/gtykusgwkr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shangyingyoupin.top/gtcqrxvyxg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.haohaochexian.top/gtoiswitxl.html

Go:   name := "Alex"; age := 20
来源：http://hz.vqdsnc.cn/gtapfnynan.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj20258888.top/gtvoueqoyz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hysaishi.cn/gtmporqggx.html

[A03] 常量定义
来源：http://hz.jinqigufen.top/gtoibigbpz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tianlin.xyz/gtkkfdvaop.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258.top/gtwsobncrz.html

JS:   const PI = 3.14159;
来源：http://hz.chenzaomai.com/gtcdblygri.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigfzy.top/gtwbanguxe.html

Java: static final double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtdmfcwekr.html

Go:   const PI = 3.14159
来源：http://hz.gotoacloud.top/gtwlgouhce.html

Ruby: PI = 3.14159
来源：http://hz.shangyingyoupin.top/gtvbsdxaqq.html

C#:   const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtehkzvdry.html

[A04] 判断变量类型
来源：http://hz.yonumen.top/gtordhrvim.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shzxlz.cn/gtcomoqwrl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ydzc1.top/gtlbapdkge.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jlsjyb.cn/gtanoitemm.html

TS:   typeof x; x instanceof Date
来源：http://hz.52xcode.cn/gttzgmndif.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhaomingkeji.xyz/gtmowstzmq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shzxlz.cn/gtskhpskfo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.316326.xyz/gtldeermli.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj20258888.top/gtmgvvrarr.html

[A05] 整数除法与取模
来源：http://hz.kuanghao11.cn/gthnkzuplk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinghuilouyu.cn/gtoosdauwu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hysaishi.cn/gtrwusppso.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ppjwa.cn/gtrstfovrs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pycfn.com/gtsjdgrxfk.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhijiandao.cn/gtdklcfyso.html

Go:   7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtkfexbxnx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhixingplan.top/gttqfgatqp.html

C#:   7 / 2; 7 % 2
来源：http://hz.birdmap.top/gthenzbegw.html

[A06] 字符串转数字
来源：http://hz.sysykeji.top/gtwvuqmrjw.html

Py:   int("42"); float("3.14")
来源：http://hz.pycfn.com/gtrxxgksvf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yuanzhike.top/gtxtumrphc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.pengpengdd.cyou/gtvonlrxyk.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhoulong.xyz/gtsppftexo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.birdmap.top/gteoippxms.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.dianchejie.cn/gtadbvhnlk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.cucudq.cn/gtasmqbdjo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hywenlv.cn/gtacaxalys.html

[A07] 数字转字符串
来源：http://hz.jiagoushi.top/gtxtvscnum.html

Py:   str(42)
来源：http://hz.hywenlv.cn/gtaoohtydg.html

PHP:  (string) 42; strval(42)
来源：http://hz.jianghu66.top/gtmdubkkbf.html

JS:   String(42); (42).toString()
来源：http://hz.guowangkeji.top/gtiuelssbh.html

TS:   String(42)
来源：http://hz.bjfxy.top/gtuazrotis.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sysykeji.top/gtpdkxvkte.html

Go:   strconv.Itoa(42)
来源：http://hz.smart0.xyz/gtfqzsxepc.html

Ruby: 42.to_s
来源：http://hz.chenjidiqi.icu/gtopzatfqf.html

C#:   42.ToString()
来源：http://hz.gzhubu.top/gtwzyfcfoz.html

[A08] 取整与四舍五入
来源：http://hz.guannengcc.top/gtqgycjvvu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.wangdashe.top/gtpimviwgz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.guowangkeji.top/gtgvxyzudt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hysaishi.cn/gtlivmrimr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ywan-chungtsiang.top/gtphykglva.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yangfankeji.com/gtizwjmdit.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yonumen.top/gtoqttmphy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jiagoushi.top/gtfwbhmjgl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jiagoushi.top/gtrztppfts.html

[A09] 绝对值与最大最小值
来源：http://hz.zhijiandao.cn/gtdbwfkkfb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ybcxt.top/gtkzshjcxe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtnhuwgpyv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhixingplan.top/gtolydnbyr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtmdolqlwx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.cdnleiting.top/gtkezpjeyk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.shanyushiyangkeji.top/gtdqwhhxmt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.nanxinkj.top/gtkbtqsgip.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yueranfly.top/gtvlsxtshg.html

[A10] 生成随机数
来源：http://hz.xuetiantiany.cn/gtnjulyfon.html

Py:   import random; random.randint(1, 100)
来源：http://hz.fzhhl.top/gtjlworbkx.html

PHP:  random_int(1, 100);
来源：http://hz.guowangkeji.top/gtmskyjnuo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hfpthk.cn/gtwpgivpat.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nwbrower.top/gtcqlxfjxz.html

Java: new Random().nextInt(100) + 1
来源：http://hz.shanyushiyangtech.top/gtwhchzdkr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.wangshuangyany.cn/gtglutajro.html

Ruby: rand(1..100)
来源：http://hz.guowangkeji.top/gttdanygkt.html

C#:   new Random().Next(1, 101)
来源：http://hz.andypj.xyz/gtveepgfws.html

[A11] 条件表达式（三元）
来源：http://hz.daxiang520.top/gtktocviuh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zdqjudy.top/gtwcpxaegs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gtcjogwqep.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gtsszcnxoe.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtfbsrpjgn.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtjezvusgx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sxryk.cn/gtrnprjlmr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.tanke756.top/gtyghxacqy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ehwqpu.com/gtmrougzll.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuanzhike.top/gtwpbjllfj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gzhubu.top/gtgpwzkgnc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.chenlongwang.top/gtyataifit.html

JS:   `Hello, ${name}!`
来源：http://hz.aibaodan.cn/gthrpxoonz.html

TS:   `Hello, ${name}!`
来源：http://hz.zhijiandao.cn/gtziwzfelx.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.redwolf501.top/gtssuvlodr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhoulong.xyz/gteuwpoima.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenzaomai.com/gtwtaqgqfp.html

C#:   $"Hello, {name}!"
来源：http://hz.bjfxy.top/gtwgqszmta.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.redwolf501.top/gtbrbksqat.html

Py:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtyezsrjhw.html

PHP:  "第一行\n第二行"
来源：http://hz.gotoacloud.top/gthaywmeln.html

JS:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtzulhocbb.html

TS:   "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtaztutqzl.html

Java: "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtxfslsplb.html

Go:   "第一行\n第二行"
来源：http://hz.fzhhl.top/gtepckataf.html

Ruby: "第一行\n第二行"
来源：http://hz.yj20258.top/gtzmdcmzrn.html

C#:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gtdawmznso.html

[A14] 注释写法
来源：http://hz.dianchejie.cn/gtclqrkdil.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.svipenyu.cn/gtirlttuku.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtbanktxua.html

JS:   // 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtaslxusny.html

TS:   // 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtjlxvxput.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.dianchejie.cn/gtkdbctftf.html

Go:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtjvcupilt.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jinyuanbaomall.cn/gtasimrafj.html


<!-- 参考信息 -->