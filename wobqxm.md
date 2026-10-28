代发 wailian999

[U81] JS：初始化项目
来源：http://hz.guowangkeji.top/gtxhbxwxam.html

npm init -y;  npm i express
来源：http://hz.tian-w.cn/gtsofqfhmz.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangkeji.top/gtzubqkmpk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhijiandao.cn/gtdyyamdjg.html

[U83] JS：ES Module 导入导出
来源：http://hz.xylfe.cn/gttbkdwpni.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hnxiangtu.top/gtqgixghyk.html

[U84] JS：CommonJS 写法
来源：http://hz.aibaodan.cn/gtrwgsqugi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhoulong.xyz/gtaeijtibs.html

[U85] JS：可选链
来源：http://hz.xuanzx.com/gtiuoindtq.html

a?.b?.c
来源：http://hz.ydzc1.top/gtzqrcukda.html

[U86] JS：空值合并
来源：http://hz.tanke756.top/gtqxvlzfjh.html

a ?? b
来源：http://hz.yuxming.cn/gtcmastbjc.html

[U87] JS：解构默认值
来源：http://hz.xingfuxueyuan.xyz/gtqsuuunqv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yueranfly.top/gtgrxiamuj.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtzywqstxp.html

{ ...a, ...b }
来源：http://hz.bjfxy.top/gtuwvmdolv.html

[U89] JS：数组去重
来源：http://hz.svipenyu.cn/gtrbtufzlc.html

[...new Set(arr)]
来源：http://hz.jinqigufen.top/gtimlbnerd.html

[U90] JS：数字数组排序
来源：http://hz.jinyuanbaomall.cn/gtzwuyztct.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtcfzlqidv.html

[U91] JS：对象键值遍历
来源：http://hz.vqdsnc.cn/gtzweccght.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtopevuybe.html

[U92] JS：深拷贝
来源：http://hz.ppjwa.cn/gtncwpdibh.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtzuwsfhii.html

[U93] JS：模板字符串
来源：http://hz.guowangkeji.top/gtyoqxapcx.html

`共 ${n} 条`
来源：http://hz.hysaishi.cn/gtjvtgbgqe.html

[U94] JS：箭头函数
来源：http://hz.gaohongyu789.top/gtundocdft.html

const double = x => x * 2;
来源：http://hz.iojbl.cn/gtqcdoirvl.html

[U95] JS：Promise 包装
来源：http://hz.ydzc1.top/gtlfpiekuv.html

new Promise((resolve, reject) => {})
来源：http://hz.meibo888.top/gtzblgnxmf.html

[U96] JS：async/await 与异常
来源：http://hz.sysykeji.top/gtvigzszse.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtpbxacdqh.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtnncyxlxv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtbwptcejo.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhaomingkeji.xyz/gtimwyzexu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xingfuxueyuan.xyz/gtbvefwxqa.html

[U99] JS：事件监听
来源：http://hz.cashguo.top/gtouwdiorw.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtstmilyyu.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gtqtojxudq.html

document.querySelector(".item")
来源：http://hz.havefunace.top/gtfbbqnajq.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtriajmlby.html

el.classList.toggle("active")
来源：http://hz.yonumen.top/gtlflifqvp.html

[U102] JS：本地存储
来源：http://hz.yuanzhike.top/gtduvkzovz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.smart0.xyz/gtlrmksoth.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gtdfpeihmu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yongpay.top/gtyhhwmjku.html

[U104] JS：防抖
来源：http://hz.shanyushiyangkeji.top/gtczzypmmo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtvkhgdbxr.html

[U105] JS：节流
来源：http://hz.pengpengdd.cyou/gtgsyyfgmm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangtech.top/gtbhitbvnq.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtqrkwwkjq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gzhubu.top/gtphwlvvvt.html

[U107] JS：数字千分位
来源：http://hz.yj202588.top/gtvabzzrgc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtqjrgweir.html

[U108] JS：随机整数
来源：http://hz.iojbl.cn/gtzeamsnir.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yonumen.top/gtarvkhhoh.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gtuqfnapcm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtfwvgfljg.html

[U110] JS：数组分块
来源：http://hz.meibo888.top/gtcrjpoxfz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnxiangtu.top/gtpqttzoon.html

[U111] JS：对象转 Map
来源：http://hz.xingfuxueyuan.xyz/gtyuwcpxhc.html

new Map(Object.entries(obj))
来源：http://hz.jinghuilouyu.cn/gtwwroqnop.html

[U112] JS：字符串补位
来源：http://hz.cdnleiting.top/gtzozqdypw.html

"7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtndyltjhm.html

[U113] JS：正则替换全部
来源：http://hz.jqgfzy.top/gtlblffeki.html

s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtytlcexlu.html

[U114] JS：JSON 深比较
来源：http://hz.gogol.net.cn/gtbjyxdton.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtakimfmtp.html

[U115] JS：生成 UUID
来源：http://hz.zhiwuduotai.top/gtfzsjdhso.html

crypto.randomUUID()
来源：http://hz.yvedp.cn/gtgzppogth.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinyuanbaomall.cn/gtyowntzhf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtbadqclfc.html

[U117] JS：单元测试
来源：http://hz.sufxvd.cn/gtqaoisdiv.html

npm i -D vitest;  npx vitest
来源：http://hz.aibaodan.cn/gtchxnzoku.html

[U118] JS：开发服务器
来源：http://hz.ivvv.top/gtyasgsrbx.html

npm i -D vite;  npx vite
来源：http://hz.guannengcc.top/gtgpyejorm.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtbgqvnvlp.html

npx vite build
来源：http://hz.dashuyun.cn/gtsuzsinja.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtazogxilu.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtxlmdhhxz.html

================================================================================
来源：http://hz.mhx1999.top/gtnztswxjc.html

统计汇总
来源：http://hz.hnxiangtu.top/gtlaxwtppd.html

================================================================================
来源：http://hz.zdqjudy.top/gtnfsjbvsc.html

按语言统计（条）：
来源：http://hz.iojbl.cn/gtgvukqwgj.html

Python ......... 252
来源：http://hz.smart0.xyz/gtedtdgkee.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gtyjllvfip.html

JavaScript ..... 252
来源：http://hz.cashguo.top/gtyecwldel.html

TypeScript ..... 212
来源：http://hz.9152youxi.cn/gtxiqqqrcd.html

Java ........... 212
来源：http://hz.aizwys.cn/gtpgsoeglr.html

Go ............. 212
来源：http://hz.hysaishi.cn/gtkojeinwv.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gthyqiwkto.html

C# ............. 212
来源：http://hz.aizwys.cn/gttzyuvxvt.html

C .............. 30
来源：http://hz.hysaishi.cn/gtxjlddstf.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gtvdjtfjsa.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gtntwhtaet.html

Bash ........... 80
来源：http://hz.hfpthk.cn/gtdzhwimyp.html

Kotlin ......... 15
来源：http://hz.vqdsnc.cn/gtfdlyeiin.html

Swift .......... 15
来源：http://hz.chenlongwang.top/gtxfbugzjz.html

Lua ............ 10
来源：http://hz.daxiang520.top/gtydfxfhsr.html

Perl ........... 10
来源：http://hz.cdnleiting.top/gtssyzgmal.html

Scala .......... 10
来源：http://hz.9152youxi.cn/gttdddzmxw.html

------------------------------------
来源：http://hz.yj20258888.top/gtrxwfiata.html

合计 ........... 2106 条
来源：http://hz.meibo888.top/gtyzlpryue.html

按章节统计：
来源：http://hz.hnqzz.top/gthrhatuyn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtqabedgfm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtbdzwbkun.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtmsjkfpgh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtuuabfdvf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.9152youxi.cn/gtuxeactpr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shangyingyoupin.top/gtnmdiwwxs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtcotnaxid.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtmeylxcmw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtmelrdssr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtxvdfzyfn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtilcmocfe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtcoatitcn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtqcwrnhur.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtvqpadhvk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tian-w.cn/gthrgicmom.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtjxtmsszr.html

Q SQL 专题                              90
来源：http://hz.tianlin.xyz/gtgheyxvak.html

R Bash 专题                             80
来源：http://hz.ybcxt.top/gtvcaewief.html

S C / C++ 专题                          60
来源：http://hz.hfpthk.cn/gtaaqqjscw.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtmsfsyijt.html

U 高频实用片段                         120
来源：http://hz.chenzaomai.com/gtdvoeeeda.html

------------------------------------
来源：http://hz.sweek.top/gtgrtupyrc.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtlqxqevnn.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtngiktwyh.html

使用提醒
来源：http://hz.ivvv.top/gtlpeyoirq.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtfhmszkrz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtxmnumzgq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigfzy.top/gtkiqeekhu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ivvv.top/gtibgiwbkb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.vqdsnc.cn/gtbpfzqpuv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtdplbdrpe.html

—— 文件结束 ——
来源：http://hz.shanyushiyangkeji.top/gtbevtzdwe.html

================================================================================
来源：http://hz.jqgufenzy.top/gthcikcuys.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangdashe.top/gtqobiickk.html

Common Programming Examples Cheat Book
来源：http://hz.nanxinkj.top/gtimlxzqjf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqopytvkp.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtmfuzoakn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zdqjudy.top/gtqjdgvhmp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.andypj.xyz/gttmhextdv.html

SQL · Bash · C · C++
来源：http://hz.ydjk.org.cn/gtamxllihp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cdnleiting.top/gtecrlxgwk.html

【使用说明】
来源：http://hz.xuanzx.com/gtdpuyxuzw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cashguo.top/gttobrrmez.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydjk.org.cn/gtephnjluu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenzaomai.com/gtbxbbvyun.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hywenlv.cn/gtesdgdbsp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shuidangran.top/gtninlxcpc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yanxiufei.cn/gtjtmxfaun.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hywenlv.cn/gtfixumxed.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zdqjudy.top/gtshczdjso.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtaxpqrxnh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cqqwz.cn/gtytzzmoby.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gotoacloud.top/gtrhbjofvt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.smart0.xyz/gtrxgfgobn.html

【文件统计】
来源：http://hz.nwbrower.top/gtxalsxrui.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.havefunace.top/gtklvjiqym.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtafmhqrnb.html

目  录
来源：http://hz.yangfankeji.com/gtcowtrxnx.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtupmukrme.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtblfvmnse.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtfuhcohyc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtryvnbdan.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hywenlv.cn/gtdudeuidm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinqigufen.top/gtngrizkvw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xingfuxueyuan.xyz/gtgvchwhgo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtbiutwrpr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhijiandao.cn/gtqhnyuiay.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtuahnnady.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.haohaochexian.top/gtrwltylgs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtfgmjqdtq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtfpdyzcfb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtrtmqnhdt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gtkbnbxopj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinqigfzy.top/gtewmwlhjg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtnjbwfukf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xylfe.cn/gtcbrjgdwf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shuidangran.top/gtomoidyya.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cucudq.cn/gtiysussip.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtknxbgwfp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtqtbqpcyo.html

================================================================================
来源：http://hz.tian-w.cn/gtdgxrajjs.html

A. 基础语法与类型
来源：http://hz.aizwys.cn/gtzfmmjcal.html

================================================================================
来源：http://hz.nanxinkj.top/gtpfzdmaqy.html

[A01] Hello World
来源：http://hz.zhaomingkeji.xyz/gthcfcqrml.html

Py:   print("Hello, World!")
来源：http://hz.zhongyouzk.top/gtbnjtqxvb.html

PHP:  echo "Hello, World!";
来源：http://hz.haohaochexian.top/gtcjsiwgyz.html

JS:   console.log("Hello, World!");
来源：http://hz.nanxinkj.top/gtrrrcvfwt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wangdashe.top/gtelbnmffj.html

Java: System.out.println("Hello, World!");
来源：http://hz.nwbrower.top/gtczpijcbu.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sxryk.cn/gtzhkkvkjl.html

Ruby: puts "Hello, World!"
来源：http://hz.quarkkingdee.top/gtsznknepp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinqigufen.top/gtoyksmzls.html

[A02] 变量声明与赋值
来源：http://hz.quarkkingdee.top/gtgchdxoxr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhaomingkeji.xyz/gtabopimxr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nwbrower.top/gtehduueuz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.daria6918.cn/gtfecnouzm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.snrcjt.cn/gtfhovswfs.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtyajhaaov.html

Go:   name := "Alex"; age := 20
来源：http://hz.cdnleiting.top/gtmkutyqnu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtxmhxcrea.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtmwduhtzn.html

[A03] 常量定义
来源：http://hz.zhongyouzk.top/gthmtzizxf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yangfankeji.com/gtlyrtsdux.html

PHP:  const PI = 3.14159;
来源：http://hz.iojbl.cn/gtfhrlvxbr.html

JS:   const PI = 3.14159;
来源：http://hz.sysykeji.top/gtryphrmoq.html

TS:   const PI: number = 3.14159;
来源：http://hz.yangfankeji.com/gtzuvkgiej.html

Java: static final double PI = 3.14159;
来源：http://hz.daxiang520.top/gteogpgqka.html

Go:   const PI = 3.14159
来源：http://hz.shangyingyoupin.top/gtuflhkaun.html

Ruby: PI = 3.14159
来源：http://hz.yj20258888.top/gtsiuvhqip.html

C#:   const double PI = 3.14159;
来源：http://hz.yonumen.top/gtqhlttvxt.html

[A04] 判断变量类型
来源：http://hz.yongpay.top/gtrdpximsh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydzc1.top/gtelnjrtjq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jqgufenzy.top/gtuuzagpee.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cqqwz.cn/gtbjplotsd.html

TS:   typeof x; x instanceof Date
来源：http://hz.sxryk.cn/gtgxxcxjax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xuanzx.com/gtnbxyvgus.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.quarkkingdee.top/gtauojjukd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gthcdfkdqi.html

C#:   x.GetType().Name; x is int
来源：http://hz.gogol.net.cn/gtyqmuzarc.html

[A05] 整数除法与取模
来源：http://hz.jiagoushi.top/gtrjlldmxm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.kuanghao11.cn/gtmbvnrpke.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hongshengwenyu.top/gtwbfdlfwa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.iojbl.cn/gtkkcqejtu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxinkj.top/gtwdumtlix.html

Java: 7 / 2; 7 % 2
来源：http://hz.iojbl.cn/gthesgxtcc.html

Go:   7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtzicjvmkj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtbhmxhijd.html

C#:   7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gthtdpuvzu.html

[A06] 字符串转数字
来源：http://hz.xuetiantiany.cn/gtwbqpbnsl.html

Py:   int("42"); float("3.14")
来源：http://hz.tian-w.cn/gtdehaohzb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.daria6918.cn/gtqgqhappc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sufxvd.cn/gtpujqsozz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.haohaochexian.top/gtaseirflc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ivvv.top/gtpkmzqhmu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.iojbl.cn/gtinxwvkgw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.quarkkingdee.top/gtggkdwout.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.tanke756.top/gtjvpvtcak.html

[A07] 数字转字符串
来源：http://hz.hnqzz.top/gtrftpuigo.html

Py:   str(42)
来源：http://hz.zhongyouzk.top/gthjxndvdc.html

PHP:  (string) 42; strval(42)
来源：http://hz.fengsongda.top/gttxaivlsk.html

JS:   String(42); (42).toString()
来源：http://hz.hnxiangtu.top/gtmwvswxxj.html

TS:   String(42)
来源：http://hz.yanxiufei.cn/gtnjuwfebr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yangfankeji.com/gtlpnypshw.html

Go:   strconv.Itoa(42)
来源：http://hz.cashguo.top/gtdxnywawl.html

Ruby: 42.to_s
来源：http://hz.aibaodan.cn/gtzjnltizz.html

C#:   42.ToString()
来源：http://hz.bjfxy.top/gtxnmvhdjv.html

[A08] 取整与四舍五入
来源：http://hz.zhengqikj.top/gtnjurjjqa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xinyue.icu/gtbxqqcsrs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ywan-chungtsiang.top/gthudgleio.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtniysdjju.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.tianlin.xyz/gtioklyewy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cdnleiting.top/gtxqyquvdv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.daxiang520.top/gtgdzwlebp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.hfpthk.cn/gtunwlbpcz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.redwolf501.top/gtqbpqxosf.html

[A09] 绝对值与最大最小值
来源：http://hz.cashguo.top/gthtesdani.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yanxiufei.cn/gtuxfpdtkj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.pycfn.com/gtfoqetmlv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtlhlgjdqg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.iojbl.cn/gtxzalanef.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.dashuyun.cn/gtskfotjgw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.haohaochexian.top/gtgonmgwss.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hnqzz.top/gtucxhmgll.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.fengsongda.top/gtrtxoumyx.html

[A10] 生成随机数
来源：http://hz.zhongyouzk.top/gtjffcclbb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.pycfn.com/gtrrsjlvkw.html

PHP:  random_int(1, 100);
来源：http://hz.kuanghao11.cn/gtyoghxcwn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yueranfly.top/gtfvrlgtrt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuxming.cn/gtwsqfqkhe.html

Java: new Random().nextInt(100) + 1
来源：http://hz.52xcode.cn/gtnocknxfg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.tian-w.cn/gtmbjlwlum.html

Ruby: rand(1..100)
来源：http://hz.ehwqpu.com/gtgoopdpdb.html

C#:   new Random().Next(1, 101)
来源：http://hz.daria6918.cn/gtwoskpmrm.html

[A11] 条件表达式（三元）
来源：http://hz.c1oappe.top/gtjmupccra.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zycfv.cn/gtklapaxoe.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cdnleiting.top/gtqkgddfkc.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtreylpjhz.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtvlhruyje.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtpkqdljug.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.dianchejie.cn/gtlsybtgij.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hammf.cn/gtyfywbvbz.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.dashuyun.cn/gtuwibwurb.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuxming.cn/gtowmuczdb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.wangdashe.top/gtgpxzqcsf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tian-w.cn/gtmqmyrbib.html

JS:   `Hello, ${name}!`
来源：http://hz.bjfxy.top/gtaectexth.html

TS:   `Hello, ${name}!`
来源：http://hz.hfpthk.cn/gtjxalbhki.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.snrcjt.cn/gtfovxhkwt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.dianchejie.cn/gtzqtxpcbk.html

Ruby: "Hello, #{name}!"
来源：http://hz.cashguo.top/gtxqzclpcm.html

C#:   $"Hello, {name}!"
来源：http://hz.xuanzx.com/gteynmvfpk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.52xcode.cn/gtvtzkzcma.html

Py:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtvfzislgt.html

PHP:  "第一行\n第二行"
来源：http://hz.xziqi.cn/gtfwmpplyk.html

JS:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtzscvqixg.html

TS:   "第一行\n第二行"
来源：http://hz.bjfxy.top/gtrtrzxhcx.html


<!-- 参考信息 -->