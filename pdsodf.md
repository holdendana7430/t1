代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.sysykeji.top/gtjjsqdqvw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.fengsongda.top/gtbjqdmwtb.html

[U84] JS：CommonJS 写法
来源：http://hz.shangyingyoupin.top/gtupvekfiq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hfpthk.cn/gtfqqcikkg.html

[U85] JS：可选链
来源：http://hz.aizwys.cn/gtdfxgvqgw.html

a?.b?.c
来源：http://hz.zhiwuduotai.top/gtzlafjfjy.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtucdzpuij.html

a ?? b
来源：http://hz.xinyue.icu/gthkhnixxx.html

[U87] JS：解构默认值
来源：http://hz.guowangkeji.top/gtwehyeuhk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daria6918.cn/gtcaslzexc.html

[U88] JS：对象展开合并
来源：http://hz.hywenlv.cn/gthlqdgndo.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gtoqnbwzxo.html

[U89] JS：数组去重
来源：http://hz.cdnleiting.top/gthicfjqva.html

[...new Set(arr)]
来源：http://hz.dianchejie.cn/gttuijwkpy.html

[U90] JS：数字数组排序
来源：http://hz.gotoacloud.top/gtcswnncur.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtokjdtbye.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtpfyskgbe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.kuanghao11.cn/gtpsifxhxm.html

[U92] JS：深拷贝
来源：http://hz.daxiang520.top/gtpwhonzkf.html

structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtezclgmmy.html

[U93] JS：模板字符串
来源：http://hz.snrcjt.cn/gtemfdwycw.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtixgofjny.html

[U94] JS：箭头函数
来源：http://hz.316326.xyz/gtobzlnspb.html

const double = x => x * 2;
来源：http://hz.nanxuanxn.top/gtkxazcosq.html

[U95] JS：Promise 包装
来源：http://hz.jinyuanbaomall.cn/gtrrpitxmc.html

new Promise((resolve, reject) => {})
来源：http://hz.chenlongwang.top/gtopesbrrf.html

[U96] JS：async/await 与异常
来源：http://hz.tian-w.cn/gtazmwrlad.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtxzcozgrk.html

[U97] JS：并发请求
来源：http://hz.zhaomingkeji.xyz/gtglkkhvmp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gttcjymyad.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtavwcorqe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhengqikj.top/gteenlsxss.html

[U99] JS：事件监听
来源：http://hz.shuidangran.top/gtcvbdfrsw.html

el.addEventListener("click", e => {})
来源：http://hz.hnxiangtu.top/gtghtsxwld.html

[U100] JS：DOM 查询
来源：http://hz.sweek.top/gtfdiwgcma.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtgqatncpf.html

[U101] JS：classList 操作
来源：http://hz.xylfe.cn/gtucttdakb.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtqysfxryf.html

[U102] JS：本地存储
来源：http://hz.hfpthk.cn/gtuborruft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xylfe.cn/gtaywlhvqt.html

[U103] JS：定时器
来源：http://hz.smart0.xyz/gtndfelztu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangkeji.top/gtgppqcena.html

[U104] JS：防抖
来源：http://hz.jqgfzy.top/gtjicbtnqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtmhanycyc.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gttnayvxus.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daria6918.cn/gtejbubvyf.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtqbqnklti.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.smart0.xyz/gtrpppdpad.html

[U107] JS：数字千分位
来源：http://hz.ivvv.top/gtgvbeibzc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.c1oappe.top/gtjezpnzcu.html

[U108] JS：随机整数
来源：http://hz.sxryk.cn/gtkmyadhzk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtibyjczmd.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtoigdqnit.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtfocdkrbc.html

[U110] JS：数组分块
来源：http://hz.jinqigfzy.top/gtamakaptn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuetiantiany.cn/gtilguizvv.html

[U111] JS：对象转 Map
来源：http://hz.aibaodan.cn/gtyhdosigd.html

new Map(Object.entries(obj))
来源：http://hz.jqgfzy.top/gthdqqngfv.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtmadwcjpa.html

"7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtnoiipewy.html

[U113] JS：正则替换全部
来源：http://hz.yanxiufei.cn/gtnshxvhiz.html

s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtmgcsndyu.html

[U114] JS：JSON 深比较
来源：http://hz.yonumen.top/gtfnaimuup.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtiprmgkvw.html

[U115] JS：生成 UUID
来源：http://hz.bjfxy.top/gteadassvg.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtzqpqhkls.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shanyushiyangtech.top/gtsjhepxfr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.meibo888.top/gttqefmpxe.html

[U117] JS：单元测试
来源：http://hz.ybcxt.top/gtmqvdcnsk.html

npm i -D vitest;  npx vitest
来源：http://hz.svipenyu.cn/gtlqtsbbyd.html

[U118] JS：开发服务器
来源：http://hz.bjfxy.top/gtqazjndmf.html

npm i -D vite;  npx vite
来源：http://hz.hfpthk.cn/gtbxhphail.html

[U119] JS：生产构建
来源：http://hz.xylfe.cn/gtrctedcay.html

npx vite build
来源：http://hz.cqqwz.cn/gtxfzkhwpq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtqzsxgfqc.html

import.meta.env.VITE_API_URL
来源：http://hz.yuanzhike.top/gtvcxawzfc.html

================================================================================
来源：http://hz.nanxinkj.top/gtapebxlsa.html

统计汇总
来源：http://hz.zhoulong.xyz/gtejzjiznt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttmwvawwd.html

按语言统计（条）：
来源：http://hz.cdnleiting.top/gtxlgtyfkf.html

Python ......... 252
来源：http://hz.snrcjt.cn/gtigidmost.html

PHP ............ 252
来源：http://hz.gzhubu.top/gtjyohyrah.html

JavaScript ..... 252
来源：http://hz.chenzaomai.com/gtedekxkck.html

TypeScript ..... 212
来源：http://hz.yuanzhike.top/gtnpjimohj.html

Java ........... 212
来源：http://hz.jqgfzy.top/gtwolrdfdt.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtyoftbjkm.html

Ruby ........... 212
来源：http://hz.c1oappe.top/gtwltqzxmm.html

C# ............. 212
来源：http://hz.tian-w.cn/gtehskzlau.html

C .............. 30
来源：http://hz.gzhubu.top/gtnazrwkag.html

C++ ............ 30
来源：http://hz.yj20258.top/gtkgdfikvm.html

SQL ............ 90
来源：http://hz.pycfn.com/gtehovwkwb.html

Bash ........... 80
来源：http://hz.tianlin.xyz/gtwfpxsgyx.html

Kotlin ......... 15
来源：http://hz.yongpay.top/gtlgagulgi.html

Swift .......... 15
来源：http://hz.vqdsnc.cn/gtqeqporjv.html

Lua ............ 10
来源：http://hz.xinyue.icu/gtlzbtqrgu.html

Perl ........... 10
来源：http://hz.aizwys.cn/gtngqhutki.html

Scala .......... 10
来源：http://hz.xuetiantiany.cn/gtmycigkeu.html

------------------------------------
来源：http://hz.yj20258.top/gtlsexkmat.html

合计 ........... 2106 条
来源：http://hz.jinqigfzy.top/gtydwrlkpc.html

按章节统计：
来源：http://hz.bjfxy.top/gtogcwtwjh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gttykiacwp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtsobhhhhf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtmupzdmsc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtebqjglsa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ywan-chungtsiang.top/gtyjftmxdj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gthoxoskbq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtfeddpwpe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtbftwkaab.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtpksgjxsa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daxiang520.top/gtjzzvtovn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtqmevnpvg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtizeefdeo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gthndszkoh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtcgndsnij.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dianchejie.cn/gtchacuith.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtmprqjjly.html

Q SQL 专题                              90
来源：http://hz.jinghuilouyu.cn/gtmalamhba.html

R Bash 专题                             80
来源：http://hz.svipenyu.cn/gtrgngmeso.html

S C / C++ 专题                          60
来源：http://hz.zhixingplan.top/gttsvfpfiw.html

T 其他语言补充                          60
来源：http://hz.aizwys.cn/gtbdoeamhz.html

U 高频实用片段                         120
来源：http://hz.yonumen.top/gtkueejedb.html

------------------------------------
来源：http://hz.gzhubu.top/gttegirnpq.html

合计                                  2106 条
来源：http://hz.jqgfzy.top/gtedbfypwv.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtevjqelhy.html

使用提醒
来源：http://hz.316326.xyz/gtijqmidcv.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtxkiirgpo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtuixjrkid.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cqqwz.cn/gtnbnrviun.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenjidiqi.icu/gtlvxdhkth.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuxming.cn/gtuzfqxxnj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hnxiangtu.top/gttzlqcfix.html

—— 文件结束 ——
来源：http://hz.haohaochexian.top/gtyxznhodz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnyclhdvw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.kuanghao11.cn/gtniblucae.html

Common Programming Examples Cheat Book
来源：http://hz.vqdsnc.cn/gtfbyoyajm.html

================================================================================
来源：http://hz.jianghu66.top/gtpsrtbkex.html

【收录内容】
来源：http://hz.pycfn.com/gtoadjnoet.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yangfankeji.com/gtxrjwycaw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ybcxt.top/gtzutlhukj.html

SQL · Bash · C · C++
来源：http://hz.cqqwz.cn/gtnrxypmgd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cashguo.top/gthdimbhib.html

【使用说明】
来源：http://hz.hnqzz.top/gtsxbfpcam.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jlsjyb.cn/gthupuuxyj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.9152youxi.cn/gtbbpkbqqd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yongpay.top/gtpwbqrvvl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ybcxt.top/gtcmbrnlfn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hysaishi.cn/gtcowepsvb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xziqi.cn/gtaykfxkrd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.daria6918.cn/gtmpksauzy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ywan-chungtsiang.top/gtwbnzrgjn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtuxlrpxkx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenzaomai.com/gtkatzryco.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yanxiufei.cn/gtztfgelpc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ydjk.org.cn/gtdhsmjkvm.html

【文件统计】
来源：http://hz.dianchejie.cn/gtozdiztuz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xylfe.cn/gtvckxgsnd.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtypwawwhp.html

目  录
来源：http://hz.chenlongwang.top/gtyepcywwy.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtecctvzge.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gtoncfvmmt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtgrrnpkjk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ehwqpu.com/gtfuivcani.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.haohaochexian.top/gtnxkyrggr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xinyue.icu/gtnydtngcq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtidjnbeye.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtwxuedaql.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gtrderkwmb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gttffknqez.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hammf.cn/gtmuieemqc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuxming.cn/gtgouaapaa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtacshbygx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtbqtxjvgd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.pengpengdd.cyou/gtfeiyzuqs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ppjwa.cn/gtfjrhlqkb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gttulczsfb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gtbidpmagv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yvedp.cn/gtfyktalza.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.chenlongwang.top/gtanfnvmpo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtqstivrfz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtxmvnnhha.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlcxiqxvk.html

A. 基础语法与类型
来源：http://hz.cdnleiting.top/gtkiyyjukp.html

================================================================================
来源：http://hz.hywenlv.cn/gtlpvuobuu.html

[A01] Hello World
来源：http://hz.shanyushiyangtech.top/gtscuqpopd.html

Py:   print("Hello, World!")
来源：http://hz.ywan-chungtsiang.top/gtefxbxedr.html

PHP:  echo "Hello, World!";
来源：http://hz.sufxvd.cn/gtxxelimdn.html

JS:   console.log("Hello, World!");
来源：http://hz.smart0.xyz/gttafdphax.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenjidiqi.icu/gtbaorhzgt.html

Java: System.out.println("Hello, World!");
来源：http://hz.kuanghao11.cn/gtwctpmxko.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.meibo888.top/gtrqgzuzmf.html

Ruby: puts "Hello, World!"
来源：http://hz.sweek.top/gtnuaiojpx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.smart0.xyz/gtvkqjkgoo.html

[A02] 变量声明与赋值
来源：http://hz.gaohongyu789.top/gtqyouztiy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ppjwa.cn/gtntwhuhkk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.cdnleiting.top/gtsmwpxuec.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.vqdsnc.cn/gtcwzrqfmb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hywenlv.cn/gtfwwbugrf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gtpcnvbwaf.html

Go:   name := "Alex"; age := 20
来源：http://hz.yongpay.top/gtntpuopvg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cdnleiting.top/gtwwwfjupx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gogol.net.cn/gtjjcidzan.html

[A03] 常量定义
来源：http://hz.sufxvd.cn/gtzvbrdtzw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj20258888.top/gtovpcahau.html

PHP:  const PI = 3.14159;
来源：http://hz.cdnleiting.top/gtztydqmwe.html

JS:   const PI = 3.14159;
来源：http://hz.mhx1999.top/gtjkrxznpa.html

TS:   const PI: number = 3.14159;
来源：http://hz.tianlin.xyz/gtuipfmodg.html

Java: static final double PI = 3.14159;
来源：http://hz.sysykeji.top/gtaptyerza.html

Go:   const PI = 3.14159
来源：http://hz.zhixingplan.top/gtwfiovmwa.html

Ruby: PI = 3.14159
来源：http://hz.hfpthk.cn/gtcvyzdjng.html

C#:   const double PI = 3.14159;
来源：http://hz.tanke756.top/gtpkbqzomh.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtayvvtzvy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gtpisndjrw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guannengcc.top/gtxeqrobzc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hfpthk.cn/gtiksbslzi.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtpqxihcqd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtgatabxwy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gtgojbtqbk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nwbrower.top/gtwdapdpin.html

C#:   x.GetType().Name; x is int
来源：http://hz.tianlin.xyz/gtczcllkax.html

[A05] 整数除法与取模
来源：http://hz.jinqigufen.top/gtzdhoktbw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yonumen.top/gtgahmkirr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xuanzx.com/gtrdyqqdzh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinqigfzy.top/gtfsngaabv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.9152youxi.cn/gtqnmlugup.html

Java: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtezoydizo.html

Go:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtvdlhvtqo.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gttzxlnqei.html

C#:   7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtccxkdfsz.html

[A06] 字符串转数字
来源：http://hz.tian-w.cn/gtucowjmwz.html

Py:   int("42"); float("3.14")
来源：http://hz.ydzc1.top/gthiatbesv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xziqi.cn/gttmowcasn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ybcxt.top/gtwsnlkkyi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gtrilunwgh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gzhubu.top/gtpfwtxgjf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ppjwa.cn/gtojzyqekf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinqigufen.top/gtqzwyabax.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhongyouzk.top/gtgxltbwvt.html

[A07] 数字转字符串
来源：http://hz.jyoumei.cn/gtxttgkbvs.html

Py:   str(42)
来源：http://hz.wangshuangyany.cn/gtzqwpykuf.html

PHP:  (string) 42; strval(42)
来源：http://hz.birdmap.top/gtekfrknza.html

JS:   String(42); (42).toString()
来源：http://hz.nanxinkj.top/gtyhpgipzd.html

TS:   String(42)
来源：http://hz.daxiang520.top/gtgcgiebgz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shanyushiyangkeji.top/gteyprtbni.html

Go:   strconv.Itoa(42)
来源：http://hz.pycfn.com/gtcnnvuzbs.html

Ruby: 42.to_s
来源：http://hz.zdqjudy.top/gteatntjbl.html

C#:   42.ToString()
来源：http://hz.gotoacloud.top/gtujdcfjll.html

[A08] 取整与四舍五入
来源：http://hz.fengsongda.top/gtiyaydjdy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yangfankeji.com/gtibvrwkqo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cdnleiting.top/gtagvctunk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.pengpengdd.cyou/gtimahtuvn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ywan-chungtsiang.top/gtyxtlsdgc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.fengsongda.top/gtnbjtwvql.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.sufxvd.cn/gtgysioehr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xuanzx.com/gtweyrurwg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.smart0.xyz/gtmiqmnvom.html

[A09] 绝对值与最大最小值
来源：http://hz.chenlongwang.top/gtwngtypfn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gtpfltsyja.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gtgatnsqml.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.guowangkeji.top/gtyzqxevan.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.pycfn.com/gtqfifmxpk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtfpzhilnz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinqigfzy.top/gtpzkxnwth.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.wangshuangyany.cn/gtydnmsqbl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.vqdsnc.cn/gthvvbapms.html

[A10] 生成随机数
来源：http://hz.wangshuangyany.cn/gtgymgnbdp.html

Py:   import random; random.randint(1, 100)
来源：http://hz.316326.xyz/gtxtxadmfs.html

PHP:  random_int(1, 100);
来源：http://hz.shanyushiyangtech.top/gtplhsamsl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hongshengwenyu.top/gtarjsuvhi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.tanke756.top/gthcajsknm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yongpay.top/gthvlnzyhb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ydjk.org.cn/gtwgapsptz.html

Ruby: rand(1..100)
来源：http://hz.yongpay.top/gtvgqreaev.html

C#:   new Random().Next(1, 101)
来源：http://hz.haohaochexian.top/gtjwhyovnm.html

[A11] 条件表达式（三元）
来源：http://hz.wangshuangyany.cn/gtjudxxxrl.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.ybcxt.top/gtoztubido.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.snrcjt.cn/gtcycqzvuh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtygzxbvva.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gtquvrqgaf.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtoxwzjwui.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.chenzaomai.com/gtjecebvqu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtfakyxhxm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gtnmszfykn.html

[A12] 字符串插值 / 格式化
来源：http://hz.ehwqpu.com/gtkutbzrro.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.redwolf501.top/gtdkuhehnv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.chenjidiqi.icu/gtugiuynbq.html

JS:   `Hello, ${name}!`
来源：http://hz.cdnleiting.top/gtwgirhtyc.html

TS:   `Hello, ${name}!`
来源：http://hz.yuxming.cn/gthiktuhtw.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yj20258888.top/gtopsgrwjk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.guowangkeji.top/gthbthsgnu.html

Ruby: "Hello, #{name}!"
来源：http://hz.ydjk.org.cn/gtbmlnmtbi.html

C#:   $"Hello, {name}!"
来源：http://hz.vqdsnc.cn/gthqvvlijl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hysaishi.cn/gtucnmpwrl.html

Py:   "第一行\n第二行"
来源：http://hz.gotoacloud.top/gtmvxhduin.html

PHP:  "第一行\n第二行"
来源：http://hz.yj202588.top/gtmhdroire.html

JS:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtreilgngd.html

TS:   "第一行\n第二行"
来源：http://hz.vqdsnc.cn/gtihjgcmtd.html

Java: "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtowbitsux.html

Go:   "第一行\n第二行"
来源：http://hz.tanke756.top/gtoyvkgwiz.html

Ruby: "第一行\n第二行"
来源：http://hz.jqgufenzy.top/gtujrivzvx.html

C#:   "第一行\n第二行"
来源：http://hz.meibo888.top/gtxeuptwcr.html


<!-- 参考信息 -->