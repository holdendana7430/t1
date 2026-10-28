代发 wailian999

[U79] PHP：静态分析
来源：http://hz.wangshuangyany.cn/gtcppuniaj.html

composer require --dev phpstan/phpstan
来源：http://hz.shanyushiyangtech.top/gtrewetoap.html

[U80] PHP：代码规范修复
来源：http://hz.316326.xyz/gtkjxykjdm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtgaogbahl.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gtsitjbcuc.html

npm init -y;  npm i express
来源：http://hz.mhx1999.top/gtwpydcotl.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtzzlpbkrw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ivvv.top/gtlhcklfib.html

[U83] JS：ES Module 导入导出
来源：http://hz.guowangkeji.top/gtbwvwvstl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.haohaochexian.top/gtlmepbkqq.html

[U84] JS：CommonJS 写法
来源：http://hz.yongpay.top/gtkywrsbnk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtklrmwwcv.html

[U85] JS：可选链
来源：http://hz.ydjk.org.cn/gtwrljzmnp.html

a?.b?.c
来源：http://hz.pengpengdd.cyou/gtzwnpggxk.html

[U86] JS：空值合并
来源：http://hz.zhixingplan.top/gtqtpjfjfn.html

a ?? b
来源：http://hz.nwbrower.top/gtvhoxlgnx.html

[U87] JS：解构默认值
来源：http://hz.sxryk.cn/gthlzcencj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sxryk.cn/gtyxcwvhcf.html

[U88] JS：对象展开合并
来源：http://hz.daria6918.cn/gtgzqolxih.html

{ ...a, ...b }
来源：http://hz.9152youxi.cn/gtcyzmmclk.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtdpapbxyj.html

[...new Set(arr)]
来源：http://hz.yonumen.top/gtktdqjgba.html

[U90] JS：数字数组排序
来源：http://hz.jinyuanbaomall.cn/gtmeubkvuh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtzrshmroe.html

[U91] JS：对象键值遍历
来源：http://hz.hongshengwenyu.top/gtxfozmuys.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sweek.top/gtpypbdhad.html

[U92] JS：深拷贝
来源：http://hz.hnxiangtu.top/gtcqscxfab.html

structuredClone(obj)
来源：http://hz.ehwqpu.com/gtymrrgbqa.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtgiwfykyy.html

`共 ${n} 条`
来源：http://hz.9152youxi.cn/gtxhydjbtd.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtkubcwqed.html

const double = x => x * 2;
来源：http://hz.gaohongyu789.top/gtqtvuhryf.html

[U95] JS：Promise 包装
来源：http://hz.ppjwa.cn/gtxbqggqkt.html

new Promise((resolve, reject) => {})
来源：http://hz.ywan-chungtsiang.top/gtrxwcentm.html

[U96] JS：async/await 与异常
来源：http://hz.xuanzx.com/gtlgyhqufn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtsiggfaae.html

[U97] JS：并发请求
来源：http://hz.zdqjudy.top/gtxseonsxe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gthszytcxi.html

[U98] JS：fetch 带 JSON
来源：http://hz.jlsjyb.cn/gtnowayzwi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.svipenyu.cn/gtkbbnmoxw.html

[U99] JS：事件监听
来源：http://hz.pycfn.com/gtedvdarsd.html

el.addEventListener("click", e => {})
来源：http://hz.quarkkingdee.top/gtauugerov.html

[U100] JS：DOM 查询
来源：http://hz.aizwys.cn/gtdaujpbuo.html

document.querySelector(".item")
来源：http://hz.gogol.net.cn/gtgxwpwuku.html

[U101] JS：classList 操作
来源：http://hz.cheryme.top/gtiwuuryum.html

el.classList.toggle("active")
来源：http://hz.dashuyun.cn/gtprincgqe.html

[U102] JS：本地存储
来源：http://hz.zhiwuduotai.top/gtraexbfqg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.meibo888.top/gtajjzucev.html

[U103] JS：定时器
来源：http://hz.jinqigufen.top/gtmetlwihj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zycfv.cn/gtnagwqoik.html

[U104] JS：防抖
来源：http://hz.hfpthk.cn/gtfeomaduu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtfgxcltsq.html

[U105] JS：节流
来源：http://hz.aizwys.cn/gtppnwynwl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydzc1.top/gtfcxrcfoq.html

[U106] JS：日期格式化
来源：http://hz.tanke756.top/gtukfopvhl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hnxiangtu.top/gtvmaebvog.html

[U107] JS：数字千分位
来源：http://hz.xinyue.icu/gtkkyapgvx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cheryme.top/gtircgxskz.html

[U108] JS：随机整数
来源：http://hz.kuanghao11.cn/gtetgotwzn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gtfeakbrtm.html

[U109] JS：数组分组
来源：http://hz.ydzc1.top/gtxjyaahxt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtcknzsjao.html

[U110] JS：数组分块
来源：http://hz.zhaomingkeji.xyz/gtnspewyky.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenzaomai.com/gtdnqrkhlk.html

[U111] JS：对象转 Map
来源：http://hz.hnqzz.top/gtfwwmlxin.html

new Map(Object.entries(obj))
来源：http://hz.gotoacloud.top/gtcigzvilu.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gtddefjjho.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtwrnrnkpa.html

[U113] JS：正则替换全部
来源：http://hz.nanxinkj.top/gtudhalxht.html

s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtlofgrdqd.html

[U114] JS：JSON 深比较
来源：http://hz.havefunace.top/gtnjkdmasa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtwvbmsaco.html

[U115] JS：生成 UUID
来源：http://hz.vqdsnc.cn/gtwcfydjrw.html

crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtelhuqlnm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tian-w.cn/gtjombejfw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.52xcode.cn/gtcpqratcg.html

[U117] JS：单元测试
来源：http://hz.dianchejie.cn/gtoikpiniv.html

npm i -D vitest;  npx vitest
来源：http://hz.bjfxy.top/gteqrzmifp.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtavehokpm.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gtrgjodjoi.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtchejptsa.html

npx vite build
来源：http://hz.zhengqikj.top/gtoywgjjmc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.316326.xyz/gtwcjwccfh.html

import.meta.env.VITE_API_URL
来源：http://hz.ppjwa.cn/gtganwjwzy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkxyeqwqr.html

统计汇总
来源：http://hz.guannengcc.top/gtfmyrtzwu.html

================================================================================
来源：http://hz.sweek.top/gtuseeosna.html

按语言统计（条）：
来源：http://hz.svipenyu.cn/gtbwjqpyko.html

Python ......... 252
来源：http://hz.nanxinkj.top/gtseihmlpq.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtypkhpuko.html

JavaScript ..... 252
来源：http://hz.sweek.top/gtgwhgtzfk.html

TypeScript ..... 212
来源：http://hz.daria6918.cn/gtdufbvzbn.html

Java ........... 212
来源：http://hz.yonumen.top/gtfyqhrdey.html

Go ............. 212
来源：http://hz.guannengcc.top/gttwnxveph.html

Ruby ........... 212
来源：http://hz.svipenyu.cn/gtmsxqbthf.html

C# ............. 212
来源：http://hz.sysykeji.top/gtmmcroiqk.html

C .............. 30
来源：http://hz.xylfe.cn/gtsowpwbrr.html

C++ ............ 30
来源：http://hz.quarkkingdee.top/gtbugcvwxa.html

SQL ............ 90
来源：http://hz.pengpengdd.cyou/gthvxvchyy.html

Bash ........... 80
来源：http://hz.aizwys.cn/gturlbkawk.html

Kotlin ......... 15
来源：http://hz.sysykeji.top/gtsisspzav.html

Swift .......... 15
来源：http://hz.shangyingyoupin.top/gtgumiigho.html

Lua ............ 10
来源：http://hz.andypj.xyz/gtflzmadbi.html

Perl ........... 10
来源：http://hz.havefunace.top/gtiuujouod.html

Scala .......... 10
来源：http://hz.mhx1999.top/gtkhlyiths.html

------------------------------------
来源：http://hz.zycfv.cn/gtlwwywhzm.html

合计 ........... 2106 条
来源：http://hz.ydzc1.top/gtxmyulqvn.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtvvdwayso.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtlpulryvv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtnctdbses.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtilpdxdtt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yuxming.cn/gtwfpzteyv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zycfv.cn/gtjcicvvnj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sysykeji.top/gtanovpdbm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtglklzzzv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtgusuhswm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtoauxvpri.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinqigfzy.top/gtsqcifkik.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtaezhepml.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtvphjtswa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtdcbqlisj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258.top/gtnitiwdmj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtnxrdhyzt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtkxlqtcva.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtmpeviokd.html

R Bash 专题                             80
来源：http://hz.yj20258888.top/gtefyigyki.html

S C / C++ 专题                          60
来源：http://hz.fzhhl.top/gtmoordkdp.html

T 其他语言补充                          60
来源：http://hz.0kj1m.cn/gtrjalhsdt.html

U 高频实用片段                         120
来源：http://hz.yj202588.top/gtspayrumk.html

------------------------------------
来源：http://hz.tianlin.xyz/gtcvbcrqnc.html

合计                                  2106 条
来源：http://hz.shzxlz.cn/gtoalpbqpv.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtkcvzeibl.html

使用提醒
来源：http://hz.zhijiandao.cn/gtcrwvnpbm.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gttdayunbq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nwbrower.top/gttzgucosa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hfpthk.cn/gtbxlmpdpg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.bjfxy.top/gtnmcatbxv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yanxiufei.cn/gtdymdjykq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yongpay.top/gtkmnqqmkj.html

—— 文件结束 ——
来源：http://hz.zhaomingkeji.xyz/gtuiarotvt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdxdrzenq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hywenlv.cn/gtrqxmjafy.html

Common Programming Examples Cheat Book
来源：http://hz.chenjidiqi.icu/gtymxpemts.html

================================================================================
来源：http://hz.zhengqikj.top/gtrhzpnkak.html

【收录内容】
来源：http://hz.hongshengwenyu.top/gtypmnejxn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jqgufenzy.top/gtjwimjbcb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.c1oappe.top/gttirsqqnq.html

SQL · Bash · C · C++
来源：http://hz.aibaodan.cn/gtzhpbqsuu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ydzc1.top/gtuqxmdgtq.html

【使用说明】
来源：http://hz.yuxming.cn/gtkxsfqhzj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhaomingkeji.xyz/gtwbmpwdzu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenlongwang.top/gtkqxailsz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.daria6918.cn/gtsnvhushz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yueranfly.top/gtuklhidtk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydzc1.top/gtlrdxdder.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yanxiufei.cn/gtgxkrhtgh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgufenzy.top/gtjctvuqhb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhongyouzk.top/gtenhmotca.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigfzy.top/gtvejlxzsj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.guowangkeji.top/gteiufdjfk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ydzc1.top/gtebbrqgdf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangshuangyany.cn/gtwpwykphh.html

【文件统计】
来源：http://hz.wangshuangyany.cn/gtqlfyudbp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.havefunace.top/gtaknknnxf.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtucfbrvvk.html

目  录
来源：http://hz.jiagoushi.top/gtnxffcbeu.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtahotfkkp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ybcxt.top/gtwscgojtq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtkviklhup.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtpflgqofw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtpbcitsji.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxuanxn.top/gtqzjbobxm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.snrcjt.cn/gtjqigcurs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yongpay.top/gtamtzisis.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtipzhlinl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.haohaochexian.top/gtwbmrwthw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtlkabucsk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtthtxotky.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtpwdgrvbv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtklrwpmki.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hongshengwenyu.top/gtkxblpedg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xziqi.cn/gtbabwmllb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gthwhcgszw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258888.top/gtbdkxgwqm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yueranfly.top/gtolnvpqve.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.fengsongda.top/gtevehxkde.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtgavdlisr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtpzfozfej.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqzllpnsy.html

A. 基础语法与类型
来源：http://hz.ehwqpu.com/gtnyyosvil.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfrhxetwr.html

[A01] Hello World
来源：http://hz.shzxlz.cn/gtorpzxqyd.html

Py:   print("Hello, World!")
来源：http://hz.smart0.xyz/gtaeuoycof.html

PHP:  echo "Hello, World!";
来源：http://hz.sweek.top/gtbqqlimkb.html

JS:   console.log("Hello, World!");
来源：http://hz.yongpay.top/gteucszqhy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jqgufenzy.top/gtklqskgmk.html

Java: System.out.println("Hello, World!");
来源：http://hz.sxryk.cn/gtppdcgijt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.snrcjt.cn/gtbvfyjttm.html

Ruby: puts "Hello, World!"
来源：http://hz.birdmap.top/gtygkizwyp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.aizwys.cn/gtvoxmidqz.html

[A02] 变量声明与赋值
来源：http://hz.shangyingyoupin.top/gtztjhllyq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jqgufenzy.top/gtvgwwjwgd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hammf.cn/gtmcpskrqc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhongyouzk.top/gtuiflxwls.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pycfn.com/gtndzbemrv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtyiujaixc.html

Go:   name := "Alex"; age := 20
来源：http://hz.zycfv.cn/gtakhshbma.html

Ruby: name = "Alex"; age = 20
来源：http://hz.wangdashe.top/gtioxcfobi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zdqjudy.top/gtowjiktwa.html

[A03] 常量定义
来源：http://hz.guowangkeji.top/gtytzilepv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.havefunace.top/gtfyporhfm.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtzojokbkb.html

JS:   const PI = 3.14159;
来源：http://hz.xziqi.cn/gtmgemzyly.html

TS:   const PI: number = 3.14159;
来源：http://hz.cheryme.top/gtbtiahrqu.html

Java: static final double PI = 3.14159;
来源：http://hz.jianghu66.top/gtzvqpdtby.html

Go:   const PI = 3.14159
来源：http://hz.aibaodan.cn/gtgyabeqgs.html

Ruby: PI = 3.14159
来源：http://hz.yj202588.top/gthevgeakd.html

C#:   const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtxzvjfvxf.html

[A04] 判断变量类型
来源：http://hz.ivvv.top/gtlfqdgkmh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhongyouzk.top/gtmryicttp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.tian-w.cn/gtgywohckp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nwbrower.top/gtffppucww.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtipenwtbq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.c1oappe.top/gtgjywjqtp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tianlin.xyz/gtguhfcmlj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jyoumei.cn/gttzezxtws.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgfzy.top/gtrafpwwgp.html

[A05] 整数除法与取模
来源：http://hz.fzhhl.top/gthvmccnnf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.9152youxi.cn/gtfvecmlxf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.smart0.xyz/gtfxehewcz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258888.top/gtlgjgedui.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtixvrbznt.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtrheozwps.html

Go:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtallwpgwh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gtehsbudzc.html

C#:   7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gtdaynvfil.html

[A06] 字符串转数字
来源：http://hz.andypj.xyz/gtlrkrlljv.html

Py:   int("42"); float("3.14")
来源：http://hz.ydjk.org.cn/gtqyjdqzpz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yuanzhike.top/gtxwhewcjv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.daria6918.cn/gtefaahwdm.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ivvv.top/gturpwhrdb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yonumen.top/gtkwqdhdyx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.smart0.xyz/gtvcpxlhlf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ppjwa.cn/gtqukdqwcg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.daria6918.cn/gtwdqyttrm.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtghyfauak.html

Py:   str(42)
来源：http://hz.cheryme.top/gtssqlimif.html

PHP:  (string) 42; strval(42)
来源：http://hz.yongpay.top/gtdrqaemml.html

JS:   String(42); (42).toString()
来源：http://hz.ydjk.org.cn/gtkzwmvirn.html

TS:   String(42)
来源：http://hz.andypj.xyz/gtddrshoby.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shanyushiyangtech.top/gtjeprtiwj.html

Go:   strconv.Itoa(42)
来源：http://hz.tianlin.xyz/gtwizcrfmt.html

Ruby: 42.to_s
来源：http://hz.daxiang520.top/gtmmeivkbx.html

C#:   42.ToString()
来源：http://hz.hysaishi.cn/gtzavdxedb.html

[A08] 取整与四舍五入
来源：http://hz.sysykeji.top/gtgahvyrdw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ehwqpu.com/gtcvcltlpu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gaohongyu789.top/gtohgbcovn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hnqzz.top/gtqjayklkn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.fzhhl.top/gtllpcirza.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.pengpengdd.cyou/gtkwnzaapd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tianlin.xyz/gtcxhkbqpt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.iojbl.cn/gtbxnvftmh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hfpthk.cn/gtgjiebnwx.html

[A09] 绝对值与最大最小值
来源：http://hz.hywenlv.cn/gtiufkywsy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aizwys.cn/gttucqapyk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenjidiqi.icu/gtrvrnazgw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtfpojgrhk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.havefunace.top/gtbhanpfny.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.gotoacloud.top/gtvgkukzqp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.fzhhl.top/gtqlvzupkq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yj20258888.top/gtdiqmjdhz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.daria6918.cn/gttfdkhdgu.html

[A10] 生成随机数
来源：http://hz.yonumen.top/gtsfklezku.html

Py:   import random; random.randint(1, 100)
来源：http://hz.snrcjt.cn/gtqihulvzx.html

PHP:  random_int(1, 100);
来源：http://hz.cqqwz.cn/gtbeovuunl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daxiang520.top/gtfrkctrwx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nanxinkj.top/gtnjvrcszj.html

Java: new Random().nextInt(100) + 1
来源：http://hz.quarkkingdee.top/gthjewxehs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.redwolf501.top/gtawinqtyo.html

Ruby: rand(1..100)
来源：http://hz.guannengcc.top/gtvccvpyhx.html

C#:   new Random().Next(1, 101)
来源：http://hz.wangdashe.top/gtuetqrvpc.html

[A11] 条件表达式（三元）
来源：http://hz.nanxinkj.top/gtaanhldls.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.ybcxt.top/gtpescrxhp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gtehnmmpxf.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtwpxhrnax.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtfcmxchkl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtgumviexi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ydjk.org.cn/gtlnfndtvc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gtvsqbgglq.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtxayvqgsl.html

[A12] 字符串插值 / 格式化
来源：http://hz.fengsongda.top/gtvenpnjaq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.316326.xyz/gtmrseodgn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.hysaishi.cn/gtrrjbzlpo.html

JS:   `Hello, ${name}!`
来源：http://hz.zhoulong.xyz/gtcbbzmbpv.html

TS:   `Hello, ${name}!`
来源：http://hz.jianghu66.top/gtkqtbfkwr.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jlsjyb.cn/gthlvjkzym.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.daria6918.cn/gtvhgylobj.html

Ruby: "Hello, #{name}!"
来源：http://hz.feifeiyinyue.top/gtrubibvuv.html

C#:   $"Hello, {name}!"
来源：http://hz.hongshengwenyu.top/gtncifjiex.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.gzhubu.top/gtgbspkmnh.html


<!-- 参考信息 -->