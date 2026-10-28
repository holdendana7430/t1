代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.havefunace.top/gtbgfyjfpb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydzc1.top/gtbjthuiwo.html

[U84] JS：CommonJS 写法
来源：http://hz.52xcode.cn/gtsdlykrbs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cashguo.top/gtbwxberaw.html

[U85] JS：可选链
来源：http://hz.chenzaomai.com/gtceeuasae.html

a?.b?.c
来源：http://hz.cashguo.top/gtlpziarxq.html

[U86] JS：空值合并
来源：http://hz.yueranfly.top/gtlrtsqhdi.html

a ?? b
来源：http://hz.pengpengdd.cyou/gtjtmsyzwq.html

[U87] JS：解构默认值
来源：http://hz.cashguo.top/gtajrpmelo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhaomingkeji.xyz/gtrdexqqvu.html

[U88] JS：对象展开合并
来源：http://hz.cheryme.top/gtgjaqeeww.html

{ ...a, ...b }
来源：http://hz.zhengqikj.top/gtpuxbqiar.html

[U89] JS：数组去重
来源：http://hz.yangfankeji.com/gtnyfoxusu.html

[...new Set(arr)]
来源：http://hz.iojbl.cn/gtjemkpjjw.html

[U90] JS：数字数组排序
来源：http://hz.zhengqikj.top/gtkbnztunq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtfitxzhgr.html

[U91] JS：对象键值遍历
来源：http://hz.cheryme.top/gtvykovhbn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ivvv.top/gtdqmphhhm.html

[U92] JS：深拷贝
来源：http://hz.tanke756.top/gtzttnolbr.html

structuredClone(obj)
来源：http://hz.dianchejie.cn/gthsejnrzc.html

[U93] JS：模板字符串
来源：http://hz.yvedp.cn/gtktanuung.html

`共 ${n} 条`
来源：http://hz.yuxming.cn/gtkgmlqvwq.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtxfsruerm.html

const double = x => x * 2;
来源：http://hz.daxiang520.top/gtrroxvetx.html

[U95] JS：Promise 包装
来源：http://hz.iojbl.cn/gtuvjctlig.html

new Promise((resolve, reject) => {})
来源：http://hz.tanke756.top/gtzwidqpbw.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtwopnpaov.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtcsfeboft.html

[U97] JS：并发请求
来源：http://hz.jqgfzy.top/gtoxdnoqkl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtpwjmhfya.html

[U98] JS：fetch 带 JSON
来源：http://hz.yongpay.top/gtgjjekgml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.feifeiyinyue.top/gtjmfwxmeg.html

[U99] JS：事件监听
来源：http://hz.chenzaomai.com/gtbbailwki.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtuwumjvhb.html

[U100] JS：DOM 查询
来源：http://hz.iojbl.cn/gtfnsddhnr.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtxotzdmsn.html

[U101] JS：classList 操作
来源：http://hz.feifeiyinyue.top/gthrcgupcf.html

el.classList.toggle("active")
来源：http://hz.xingfuxueyuan.xyz/gtdgbcdiue.html

[U102] JS：本地存储
来源：http://hz.zhaomingkeji.xyz/gtejpcfmxq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtwmmtfnhw.html

[U103] JS：定时器
来源：http://hz.jqgufenzy.top/gtpfydfjlb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.vqdsnc.cn/gtzljfqzna.html

[U104] JS：防抖
来源：http://hz.jianghu66.top/gtfezzowwj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtcdbkxysq.html

[U105] JS：节流
来源：http://hz.9152youxi.cn/gtschojrhu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jqgfzy.top/gtarqfmqqg.html

[U106] JS：日期格式化
来源：http://hz.hongshengwenyu.top/gtkqgedysn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtjhycmeiy.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtmxznojlw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.birdmap.top/gthxnycdox.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtodvercsm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj202588.top/gtqzvettek.html

[U109] JS：数组分组
来源：http://hz.xinyue.icu/gtaauyiwtf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtatpjoeaw.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtewzbjyev.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hammf.cn/gtnuyickoz.html

[U111] JS：对象转 Map
来源：http://hz.gotoacloud.top/gtmrcfohwc.html

new Map(Object.entries(obj))
来源：http://hz.wangdashe.top/gtarxkyjqy.html

[U112] JS：字符串补位
来源：http://hz.hnxiangtu.top/gtzwdmdhgq.html

"7".padStart(3, "0")
来源：http://hz.meibo888.top/gtneujgpnc.html

[U113] JS：正则替换全部
来源：http://hz.52xcode.cn/gtpmzaydae.html

s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtyidzlqwv.html

[U114] JS：JSON 深比较
来源：http://hz.gogol.net.cn/gtmbsdbtcv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhoulong.xyz/gtegrazvhi.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtjqfobpwv.html

crypto.randomUUID()
来源：http://hz.mhx1999.top/gthjdlqsyf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtgljmkprr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gaohongyu789.top/gtwhgvvxvp.html

[U117] JS：单元测试
来源：http://hz.gotoacloud.top/gtfeuqospe.html

npm i -D vitest;  npx vitest
来源：http://hz.chenzaomai.com/gtlifimnyb.html

[U118] JS：开发服务器
来源：http://hz.zhiwuduotai.top/gtbrdxqhkh.html

npm i -D vite;  npx vite
来源：http://hz.nwbrower.top/gtnambpfbq.html

[U119] JS：生产构建
来源：http://hz.yonumen.top/gtezosjdqt.html

npx vite build
来源：http://hz.jqgufenzy.top/gtqwbwnxwp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.aizwys.cn/gtfqaenasl.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtxxfwnpwt.html

================================================================================
来源：http://hz.yangfankeji.com/gtfmxwkkcl.html

统计汇总
来源：http://hz.jinqigufen.top/gtaobzlmis.html

================================================================================
来源：http://hz.vqdsnc.cn/gttgvztqas.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gtkvvoepih.html

Python ......... 252
来源：http://hz.svipenyu.cn/gtqfmmawkp.html

PHP ............ 252
来源：http://hz.gzhubu.top/gtybrhitso.html

JavaScript ..... 252
来源：http://hz.yongpay.top/gtcqcxklfp.html

TypeScript ..... 212
来源：http://hz.jinyuanbaomall.cn/gtdkmaqgmx.html

Java ........... 212
来源：http://hz.sysykeji.top/gtaeqfociv.html

Go ............. 212
来源：http://hz.jyoumei.cn/gtiaokgqub.html

Ruby ........... 212
来源：http://hz.hongshengwenyu.top/gtlrkfrgpt.html

C# ............. 212
来源：http://hz.iojbl.cn/gtuuyavnny.html

C .............. 30
来源：http://hz.zhiwuduotai.top/gtjwdcsvjs.html

C++ ............ 30
来源：http://hz.redwolf501.top/gtltstfoou.html

SQL ............ 90
来源：http://hz.ybcxt.top/gtqxzteqpx.html

Bash ........... 80
来源：http://hz.xinyue.icu/gtikofxvun.html

Kotlin ......... 15
来源：http://hz.gogol.net.cn/gtitpdxkcu.html

Swift .......... 15
来源：http://hz.aibaodan.cn/gtgwmvqkni.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtbzmteimq.html

Perl ........... 10
来源：http://hz.316326.xyz/gtextdicae.html

Scala .......... 10
来源：http://hz.yanxiufei.cn/gtzonvfbcw.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtwmadehal.html

合计 ........... 2106 条
来源：http://hz.yuanzhike.top/gtdwwcsrxj.html

按章节统计：
来源：http://hz.wangshuangyany.cn/gtgnvwtipe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtupwxqron.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtuxvdzrvx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtnblgpppb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtqkyqppgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nanxuanxn.top/gtcqhurvgq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtnhoojojb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtenemezcd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtwzavjabq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtaacmqijb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtoppsgzsn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtlggtgydj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtckmacvxi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtwawihuaz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtgbzxujhl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yuanzhike.top/gtuvbfreuq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtaohklcqd.html

Q SQL 专题                              90
来源：http://hz.yonumen.top/gtacfyuvzs.html

R Bash 专题                             80
来源：http://hz.gogol.net.cn/gtsmyltlkr.html

S C / C++ 专题                          60
来源：http://hz.ydjk.org.cn/gtxdkhanyz.html

T 其他语言补充                          60
来源：http://hz.nanxuanxn.top/gtznldifdo.html

U 高频实用片段                         120
来源：http://hz.9152youxi.cn/gtsfkqtbol.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtddrahleq.html

合计                                  2106 条
来源：http://hz.zhoulong.xyz/gtojgdnjto.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtqukplmsw.html

使用提醒
来源：http://hz.9152youxi.cn/gtbbpvtdim.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtgrgdezep.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hywenlv.cn/gtpejllhnr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenjidiqi.icu/gtknkylorb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xinyue.icu/gtjdnfpdli.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.52xcode.cn/gtxyozkexc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj20258.top/gtinheqfzt.html

—— 文件结束 ——
来源：http://hz.zycfv.cn/gthdlkqwzl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtavlayjve.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuanzhike.top/gtdlmmzdcj.html

Common Programming Examples Cheat Book
来源：http://hz.yvedp.cn/gtyllrbkaw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzxhsorqk.html

【收录内容】
来源：http://hz.andypj.xyz/gtuiqipjpo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guowangkeji.top/gtlafpxnik.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yongpay.top/gtzunfyngu.html

SQL · Bash · C · C++
来源：http://hz.snrcjt.cn/gtbfksgvyu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.svipenyu.cn/gtwlmhtsqg.html

【使用说明】
来源：http://hz.yongpay.top/gtqmjrdolt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hfpthk.cn/gtsxrslkho.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.bjfxy.top/gtjamzzmjv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.feifeiyinyue.top/gtuzqyzuwy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aibaodan.cn/gtejkcqgyf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sufxvd.cn/gtmjurjkgv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtoeklmrxj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtzubduftm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sweek.top/gtohnrvond.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.feifeiyinyue.top/gtneiasmzf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtuarliigz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinghuilouyu.cn/gteieqrvxw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sufxvd.cn/gtzmnsgxnh.html

【文件统计】
来源：http://hz.jqgufenzy.top/gtvareesms.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cashguo.top/gtoybyiqlu.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtcyaqiarh.html

目  录
来源：http://hz.chenjidiqi.icu/gtfrgdzifj.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtztbgjbly.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pengpengdd.cyou/gtovqzwqos.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtgixxdirv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtsciidcvb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtqthfjsps.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.chenzaomai.com/gtiqaujqmw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj20258.top/gtbdnsmjhu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtdeszbhip.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shuidangran.top/gtxzlnmzsw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtmhwhdici.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cdnleiting.top/gtsbdxxmpg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtmdycnrve.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtyuqquiot.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtqqpeyjto.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangshuangyany.cn/gtonwpturo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aizwys.cn/gtpgwzcbpj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtyjanapov.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.chenzaomai.com/gtcgomceem.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ivvv.top/gtuxrsdovz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.pengpengdd.cyou/gtmucwbjfv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtdkmeelgd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtzhwkmgmu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfoblgbnj.html

A. 基础语法与类型
来源：http://hz.gogol.net.cn/gtseadetkc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtoxanrlhc.html

[A01] Hello World
来源：http://hz.xziqi.cn/gtvypaicil.html

Py:   print("Hello, World!")
来源：http://hz.xylfe.cn/gtqwnucjps.html

PHP:  echo "Hello, World!";
来源：http://hz.gzhubu.top/gtpbwsmmts.html

JS:   console.log("Hello, World!");
来源：http://hz.aibaodan.cn/gthvzvuwmy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.daria6918.cn/gtncnepybe.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gtnxdhvixr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangdashe.top/gttptazjjn.html

Ruby: puts "Hello, World!"
来源：http://hz.fengsongda.top/gtxpovadca.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yanxiufei.cn/gtocisjpmw.html

[A02] 变量声明与赋值
来源：http://hz.kuanghao11.cn/gtikfuqafm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhoulong.xyz/gtxzsfqhfi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hfpthk.cn/gtursfxjmo.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenjidiqi.icu/gtjnzetvuj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gtknkvtpmn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jyoumei.cn/gtlmirjesk.html

Go:   name := "Alex"; age := 20
来源：http://hz.zdqjudy.top/gtvoawgcdm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.birdmap.top/gtmbltswlt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.haohaochexian.top/gtkzicvecg.html

[A03] 常量定义
来源：http://hz.feifeiyinyue.top/gtgpmgwulr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jqgfzy.top/gtjntnfjhl.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtchppphwz.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gtkwzekbmi.html

TS:   const PI: number = 3.14159;
来源：http://hz.yj20258888.top/gttdplbvsj.html

Java: static final double PI = 3.14159;
来源：http://hz.cheryme.top/gtbbmdudqn.html

Go:   const PI = 3.14159
来源：http://hz.jlsjyb.cn/gthpkqaeqa.html

Ruby: PI = 3.14159
来源：http://hz.yonumen.top/gtqqaqgjkz.html

C#:   const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gthxqcwtor.html

[A04] 判断变量类型
来源：http://hz.c1oappe.top/gtvomtmsxj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhaomingkeji.xyz/gtmjuszdyi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.smart0.xyz/gtvlbhtpbu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.9152youxi.cn/gtccedswfr.html

TS:   typeof x; x instanceof Date
来源：http://hz.gotoacloud.top/gtoypwcscm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xinyue.icu/gtkhpqpdmt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxinkj.top/gthzufiqyh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tanke756.top/gtvczakhzl.html

C#:   x.GetType().Name; x is int
来源：http://hz.xinyue.icu/gtyrhheeno.html

[A05] 整数除法与取模
来源：http://hz.zhongyouzk.top/gtzoogcwcd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhiwuduotai.top/gtvymqdcro.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.chenzaomai.com/gtmalgtuwq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinqigufen.top/gtddvptfdv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sysykeji.top/gtcemjntcq.html

Java: 7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtinvbjlpt.html

Go:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtbkfyqdte.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtnynlrgen.html

C#:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtpuxhelcs.html

[A06] 字符串转数字
来源：http://hz.feifeiyinyue.top/gtklvshgdu.html

Py:   int("42"); float("3.14")
来源：http://hz.xuanzx.com/gtmabyeeop.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.wangdashe.top/gtxjnpbftu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.haohaochexian.top/gtptmizpyu.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ywan-chungtsiang.top/gtfgzzsosj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ydjk.org.cn/gtimnogudy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.nanxinkj.top/gtigzbmtjj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.mhx1999.top/gtwhezsavd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.chenzaomai.com/gtnvlxltsq.html

[A07] 数字转字符串
来源：http://hz.zhaomingkeji.xyz/gtaigxnnla.html

Py:   str(42)
来源：http://hz.yj20258.top/gtwegeobxx.html

PHP:  (string) 42; strval(42)
来源：http://hz.mhx1999.top/gtplxeajym.html

JS:   String(42); (42).toString()
来源：http://hz.zhongyouzk.top/gtydrzsdtp.html

TS:   String(42)
来源：http://hz.jqgufenzy.top/gtudmibvmo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shuidangran.top/gtvovkptwf.html

Go:   strconv.Itoa(42)
来源：http://hz.zhixingplan.top/gthxdtahcp.html

Ruby: 42.to_s
来源：http://hz.gotoacloud.top/gtnlpwigqz.html

C#:   42.ToString()
来源：http://hz.sweek.top/gtqnaasyit.html

[A08] 取整与四舍五入
来源：http://hz.chenzaomai.com/gteblokcsd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hfpthk.cn/gttcpbqjlu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.aizwys.cn/gtghnpcjsm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.fzhhl.top/gtcuhgnbwr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ppjwa.cn/gtrkkcjbvo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.bjfxy.top/gtlixlryvp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hfpthk.cn/gtugifpmml.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ivvv.top/gtwwwdrxic.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.dashuyun.cn/gtwglxreuy.html

[A09] 绝对值与最大最小值
来源：http://hz.shangyingyoupin.top/gtnmvosjqe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.pycfn.com/gtkfzucajj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtwijagcpk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hfpthk.cn/gtqtnxruoy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gaohongyu789.top/gtfvaoirim.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.haohaochexian.top/gtwktkuedm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.pycfn.com/gtwrsfaynk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shanyushiyangtech.top/gtbeerqqbb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ybcxt.top/gtzizcaqkb.html

[A10] 生成随机数
来源：http://hz.andypj.xyz/gtqafuztem.html

Py:   import random; random.randint(1, 100)
来源：http://hz.chenzaomai.com/gtcwsdgixm.html

PHP:  random_int(1, 100);
来源：http://hz.jqgfzy.top/gtevjoqggj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhiwuduotai.top/gtubjeaxqc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangshuangyany.cn/gtpndldeam.html

Java: new Random().nextInt(100) + 1
来源：http://hz.sxryk.cn/gtfhhkhnpg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xuanzx.com/gtnldhmpwb.html

Ruby: rand(1..100)
来源：http://hz.yueranfly.top/gtlwlxapvw.html

C#:   new Random().Next(1, 101)
来源：http://hz.hnqzz.top/gtoxtvrghw.html

[A11] 条件表达式（三元）
来源：http://hz.jqgufenzy.top/gtcirxqtcx.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.andypj.xyz/gthdisstiy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtbffrjfja.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtlwocnqfj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gthwxwbock.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtiffcajtm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yueranfly.top/gtnjqzvcrc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtcbmrzfyo.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtqwpkoqtp.html

[A12] 字符串插值 / 格式化
来源：http://hz.tianlin.xyz/gtqrontbtp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hnqzz.top/gtnfrmrtvu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ppjwa.cn/gtrvmenudp.html

JS:   `Hello, ${name}!`
来源：http://hz.jinqigfzy.top/gtlqipyafa.html

TS:   `Hello, ${name}!`
来源：http://hz.dianchejie.cn/gtbpfmlouy.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.52xcode.cn/gtlruxzrzq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.chenlongwang.top/gtoqvtvkus.html

Ruby: "Hello, #{name}!"
来源：http://hz.shuidangran.top/gtdarbcoty.html

C#:   $"Hello, {name}!"
来源：http://hz.yueranfly.top/gtvgyzcsam.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xuetiantiany.cn/gtmijxxiws.html

Py:   "第一行\n第二行"
来源：http://hz.daxiang520.top/gtufyaijar.html

PHP:  "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtknwqbbej.html

JS:   "第一行\n第二行"
来源：http://hz.jqgufenzy.top/gtaxkkstis.html

TS:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gtnirnnmto.html

Java: "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtsvotjper.html

Go:   "第一行\n第二行"
来源：http://hz.jianghu66.top/gtahckdqgd.html

Ruby: "第一行\n第二行"
来源：http://hz.c1oappe.top/gtalytkepf.html

C#:   "第一行\n第二行"
来源：http://hz.sufxvd.cn/gtxgbaaczp.html


<!-- 参考信息 -->