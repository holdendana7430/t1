代发 wailian999

[U81] JS：初始化项目
来源：http://hz.sysykeji.top/gtcbwlkubn.html

npm init -y;  npm i express
来源：http://hz.xinyue.icu/gtfwdyfurx.html

[U82] JS：package.json 脚本
来源：http://hz.shuidangran.top/gtpcldopbg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnxiangtu.top/gtkishbkfl.html

[U83] JS：ES Module 导入导出
来源：http://hz.yonumen.top/gtesflircx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xinyue.icu/gtdhfsqmed.html

[U84] JS：CommonJS 写法
来源：http://hz.zhongyouzk.top/gtswktpjfg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yueranfly.top/gtyvsptqyu.html

[U85] JS：可选链
来源：http://hz.zhaomingkeji.xyz/gtjukhlzjd.html

a?.b?.c
来源：http://hz.feifeiyinyue.top/gtlmlrghbz.html

[U86] JS：空值合并
来源：http://hz.redwolf501.top/gtjfnnebgw.html

a ?? b
来源：http://hz.cheryme.top/gtmhrpdycn.html

[U87] JS：解构默认值
来源：http://hz.yj20258.top/gttjhthagl.html

const { a = 1, b = 2 } = obj;
来源：http://hz.dashuyun.cn/gtdeszjgtl.html

[U88] JS：对象展开合并
来源：http://hz.jyoumei.cn/gtsfjpalet.html

{ ...a, ...b }
来源：http://hz.cheryme.top/gtpbazmmws.html

[U89] JS：数组去重
来源：http://hz.zhengqikj.top/gtymvunvqx.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtmpompqym.html

[U90] JS：数字数组排序
来源：http://hz.jqgfzy.top/gtvyrykjnl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtnwrcoczw.html

[U91] JS：对象键值遍历
来源：http://hz.yvedp.cn/gtvgkchuas.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinyuanbaomall.cn/gtxdhnrujk.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gtoglidvhm.html

structuredClone(obj)
来源：http://hz.dianchejie.cn/gtkvkqhpug.html

[U93] JS：模板字符串
来源：http://hz.bjfxy.top/gtdpktgcvz.html

`共 ${n} 条`
来源：http://hz.daxiang520.top/gtmyyhvhjo.html

[U94] JS：箭头函数
来源：http://hz.xinyue.icu/gtehxsnrej.html

const double = x => x * 2;
来源：http://hz.sxryk.cn/gtpxwurdwt.html

[U95] JS：Promise 包装
来源：http://hz.nanxinkj.top/gtfvvkelxh.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtmtqcpxwo.html

[U96] JS：async/await 与异常
来源：http://hz.sysykeji.top/gtzmxgddwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydzc1.top/gtahxhbkdu.html

[U97] JS：并发请求
来源：http://hz.svipenyu.cn/gtafhrqjhz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtqxbuohvg.html

[U98] JS：fetch 带 JSON
来源：http://hz.tian-w.cn/gtfggyoxkk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.wangshuangyany.cn/gtefssxllq.html

[U99] JS：事件监听
来源：http://hz.yueranfly.top/gtmigebcpz.html

el.addEventListener("click", e => {})
来源：http://hz.cucudq.cn/gtctyoivjg.html

[U100] JS：DOM 查询
来源：http://hz.zhengqikj.top/gtipisoypd.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gtdxuqeigu.html

[U101] JS：classList 操作
来源：http://hz.yvedp.cn/gtvqwnahzm.html

el.classList.toggle("active")
来源：http://hz.wangshuangyany.cn/gtaufbmtgw.html

[U102] JS：本地存储
来源：http://hz.jinghuilouyu.cn/gtzknoydiy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.birdmap.top/gtyephnshj.html

[U103] JS：定时器
来源：http://hz.shangyingyoupin.top/gtnjocszxu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.birdmap.top/gtcqscibrj.html

[U104] JS：防抖
来源：http://hz.yueranfly.top/gtxglkmgpt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gthhwvkrmj.html

[U105] JS：节流
来源：http://hz.9152youxi.cn/gtqqauinpz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.316326.xyz/gticirubdo.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtzorgtrfc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tian-w.cn/gtgbodpoun.html

[U107] JS：数字千分位
来源：http://hz.jiagoushi.top/gtfwtjbnkx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.haohaochexian.top/gtwtpxkoha.html

[U108] JS：随机整数
来源：http://hz.xuanzx.com/gtrdzxnogn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yuanzhike.top/gtvltlvgss.html

[U109] JS：数组分组
来源：http://hz.yanxiufei.cn/gtfkbfhopq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangshuangyany.cn/gthifhbcgt.html

[U110] JS：数组分块
来源：http://hz.tanke756.top/gtduymdosd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shangyingyoupin.top/gtyxxqcxxu.html

[U111] JS：对象转 Map
来源：http://hz.jiagoushi.top/gticitpwxr.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtcsptnlfn.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtnywhrlns.html

"7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtxsbcefca.html

[U113] JS：正则替换全部
来源：http://hz.hysaishi.cn/gthzoinxvw.html

s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtxzyrbber.html

[U114] JS：JSON 深比较
来源：http://hz.zhaomingkeji.xyz/gtpfjmpvkp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtegbfldnk.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtnovjrlxm.html

crypto.randomUUID()
来源：http://hz.yj202588.top/gtvbikbgdh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtugdbttsm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtkefqmbxi.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtocrhktox.html

npm i -D vitest;  npx vitest
来源：http://hz.gogol.net.cn/gtgwpidzdp.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtbuvfwkot.html

npm i -D vite;  npx vite
来源：http://hz.zycfv.cn/gtxdpskjbd.html

[U119] JS：生产构建
来源：http://hz.redwolf501.top/gtaluwuvua.html

npx vite build
来源：http://hz.haohaochexian.top/gtqnkqckcj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hongshengwenyu.top/gtyngblaag.html

import.meta.env.VITE_API_URL
来源：http://hz.jyoumei.cn/gtmggziwzi.html

================================================================================
来源：http://hz.snrcjt.cn/gtrznfiihm.html

统计汇总
来源：http://hz.havefunace.top/gtesgdcjjw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtldpynelb.html

按语言统计（条）：
来源：http://hz.meibo888.top/gtmxjunrws.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtudpucakg.html

PHP ............ 252
来源：http://hz.cdnleiting.top/gtlsmzzhjj.html

JavaScript ..... 252
来源：http://hz.jyoumei.cn/gttlghvjdv.html

TypeScript ..... 212
来源：http://hz.mhx1999.top/gtkclwkasl.html

Java ........... 212
来源：http://hz.c1oappe.top/gtgkkpaocv.html

Go ............. 212
来源：http://hz.sxryk.cn/gtfqvwkdhr.html

Ruby ........... 212
来源：http://hz.fzhhl.top/gtepsqzbbb.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gtqksktgeg.html

C .............. 30
来源：http://hz.mhx1999.top/gtbmuzgtdn.html

C++ ............ 30
来源：http://hz.ehwqpu.com/gtwucmkmin.html

SQL ............ 90
来源：http://hz.daxiang520.top/gtsvatxppw.html

Bash ........... 80
来源：http://hz.xuanzx.com/gtatruyxjk.html

Kotlin ......... 15
来源：http://hz.xingfuxueyuan.xyz/gtiuojyict.html

Swift .......... 15
来源：http://hz.redwolf501.top/gtrbcbehtn.html

Lua ............ 10
来源：http://hz.guannengcc.top/gtavbvnaor.html

Perl ........... 10
来源：http://hz.yuxming.cn/gthsmsuqqx.html

Scala .......... 10
来源：http://hz.haohaochexian.top/gtmsjciozu.html

------------------------------------
来源：http://hz.quarkkingdee.top/gturothiyy.html

合计 ........... 2106 条
来源：http://hz.yj20258.top/gtllrknfxe.html

按章节统计：
来源：http://hz.sxryk.cn/gtdxhnaywa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hfpthk.cn/gtixvwyrcd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtzechncpu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtcpwkbarr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gturraptdd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shanyushiyangtech.top/gtssuvmccn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gteiwkrtpq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtghuazrpf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gtildiqntw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtdnhbkqdv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtbkjgmann.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtzrqawigt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtmlwicbhf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtsxfowunh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtxkwpflws.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.kuanghao11.cn/gtgzaxheez.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtrlvsqblv.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtkmnjbftq.html

R Bash 专题                             80
来源：http://hz.daxiang520.top/gtfknphcmg.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtpcuckrra.html

T 其他语言补充                          60
来源：http://hz.chenjidiqi.icu/gtbgcxwjca.html

U 高频实用片段                         120
来源：http://hz.ppjwa.cn/gtzfxrnyct.html

------------------------------------
来源：http://hz.zhixingplan.top/gtxujmkkfh.html

合计                                  2106 条
来源：http://hz.cqqwz.cn/gtgjosrjmu.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtiiahgzvv.html

使用提醒
来源：http://hz.quarkkingdee.top/gtneihfurt.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtrzhwgakf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtywpupxgi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yj202588.top/gtjdavowif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtsnidtwqy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhaomingkeji.xyz/gtonaofnvf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hongshengwenyu.top/gtyoqktpoq.html

—— 文件结束 ——
来源：http://hz.ywan-chungtsiang.top/gtpquomgix.html

================================================================================
来源：http://hz.mhx1999.top/gtzaraoubg.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hammf.cn/gtugfufnmf.html

Common Programming Examples Cheat Book
来源：http://hz.shzxlz.cn/gtxwdidako.html

================================================================================
来源：http://hz.gzhubu.top/gtmtwayyry.html

【收录内容】
来源：http://hz.jianghu66.top/gtitqciyqr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.52xcode.cn/gtyuaavidf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shangyingyoupin.top/gtdmabcexn.html

SQL · Bash · C · C++
来源：http://hz.52xcode.cn/gtudmktcwz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenjidiqi.icu/gtkdlrgsgy.html

【使用说明】
来源：http://hz.redwolf501.top/gtwvlmkmyt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nanxuanxn.top/gtkucyrhcn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daria6918.cn/gthxeuepbv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jqgufenzy.top/gtaxxwqehr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yanxiufei.cn/gtvivbehqw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.c1oappe.top/gtuejgyeyk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhixingplan.top/gtblrhijoj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dianchejie.cn/gtzasvgoir.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenjidiqi.icu/gtouxnztmr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sxryk.cn/gtwpwtyozw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.aibaodan.cn/gttiqomyxr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shuidangran.top/gtxoihzwbg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ppjwa.cn/gtztxhvglb.html

【文件统计】
来源：http://hz.svipenyu.cn/gtuemtocpo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj20258.top/gtuvkokgko.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtijqwibmo.html

目  录
来源：http://hz.hfpthk.cn/gtfzdfdhrr.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gtvdxfmnfk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.gzhubu.top/gtrloxqdft.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtoztiulne.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtfleflujj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtfjalektx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ppjwa.cn/gtnosnfqqv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.nanxuanxn.top/gtgxztyugp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.kuanghao11.cn/gthkoraxxr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.fzhhl.top/gtdtupibgn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtiakvdodh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtcpanyued.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtnnrcyubn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtvnxnloau.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtxkpbacvc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yvedp.cn/gtecasitmi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cucudq.cn/gtyucfkzmi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtdkvaszlk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fengsongda.top/gtuchhpeke.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yueranfly.top/gtekbljxpq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinyuanbaomall.cn/gtmlijkxue.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gttpmuowse.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gthfypzwdi.html

================================================================================
来源：http://hz.zhengqikj.top/gtwoxjfnsw.html

A. 基础语法与类型
来源：http://hz.tanke756.top/gtjlgonbzp.html

================================================================================
来源：http://hz.yvedp.cn/gtofejflip.html

[A01] Hello World
来源：http://hz.shzxlz.cn/gtihelvinl.html

Py:   print("Hello, World!")
来源：http://hz.dianchejie.cn/gtqytrqkfh.html

PHP:  echo "Hello, World!";
来源：http://hz.gaohongyu789.top/gtjawibdci.html

JS:   console.log("Hello, World!");
来源：http://hz.gotoacloud.top/gtccsvjeyy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.iojbl.cn/gtwzlzcsat.html

Java: System.out.println("Hello, World!");
来源：http://hz.sxryk.cn/gthnxkiurh.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hysaishi.cn/gtfyrddutj.html

Ruby: puts "Hello, World!"
来源：http://hz.mhx1999.top/gtooobigcp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhijiandao.cn/gtfuneagzo.html

[A02] 变量声明与赋值
来源：http://hz.dianchejie.cn/gtokfvbkxb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.fzhhl.top/gtmhmboord.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tanke756.top/gttxqgwlit.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jianghu66.top/gthgnogsjm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pycfn.com/gtjhwsdqrj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.52xcode.cn/gtywdrdvvn.html

Go:   name := "Alex"; age := 20
来源：http://hz.hysaishi.cn/gtcgoqlbkr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.c1oappe.top/gtwcxncpzb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.vqdsnc.cn/gtjhdunjeg.html

[A03] 常量定义
来源：http://hz.c1oappe.top/gtavrcvflq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cucudq.cn/gtdgsvxrcn.html

PHP:  const PI = 3.14159;
来源：http://hz.gotoacloud.top/gtmuzmhxyp.html

JS:   const PI = 3.14159;
来源：http://hz.jianghu66.top/gtcnkkhqry.html

TS:   const PI: number = 3.14159;
来源：http://hz.zdqjudy.top/gttjefarqz.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtdlqtclge.html

Go:   const PI = 3.14159
来源：http://hz.cashguo.top/gtjmacggjf.html

Ruby: PI = 3.14159
来源：http://hz.jqgufenzy.top/gthjfieynl.html

C#:   const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtljtkgjfe.html

[A04] 判断变量类型
来源：http://hz.gzhubu.top/gtjilxateo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigufen.top/gtquwmakht.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.wangdashe.top/gtxiuaudbs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nanxinkj.top/gtnstfxnbl.html

TS:   typeof x; x instanceof Date
来源：http://hz.haohaochexian.top/gtfndpuqau.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinghuilouyu.cn/gtkrwssxlg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ydzc1.top/gtyeumiitm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gtwnqtdfqr.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtmwzxazxo.html

[A05] 整数除法与取模
来源：http://hz.ydjk.org.cn/gthyqpgtvq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhaomingkeji.xyz/gtpqiakloc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.bjfxy.top/gtyhzvbyyr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nwbrower.top/gtkfwcnvmm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhixingplan.top/gthsvpkaxc.html

Java: 7 / 2; 7 % 2
来源：http://hz.redwolf501.top/gtbifzkgsk.html

Go:   7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtdkabkzzc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gtjzhbwqnu.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gttgzbxpyn.html

[A06] 字符串转数字
来源：http://hz.chenlongwang.top/gtkvbflbzh.html

Py:   int("42"); float("3.14")
来源：http://hz.kuanghao11.cn/gtuaswjfcw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.birdmap.top/gtbazsoqch.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jlsjyb.cn/gtlokqeaqp.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuetiantiany.cn/gtngfjssjx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shanyushiyangtech.top/gtpwlicttj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinqigfzy.top/gttzhjebob.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.guannengcc.top/gtfcjlvxwe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinqigufen.top/gtzxbfykbl.html

[A07] 数字转字符串
来源：http://hz.ehwqpu.com/gtlrlzzray.html

Py:   str(42)
来源：http://hz.zhaomingkeji.xyz/gteocciifa.html

PHP:  (string) 42; strval(42)
来源：http://hz.yj20258888.top/gtfcoftdqw.html

JS:   String(42); (42).toString()
来源：http://hz.fzhhl.top/gtelhdxluz.html

TS:   String(42)
来源：http://hz.fengsongda.top/gtudlazzwr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zycfv.cn/gtvuugrinw.html

Go:   strconv.Itoa(42)
来源：http://hz.wangdashe.top/gtwecljvki.html

Ruby: 42.to_s
来源：http://hz.tian-w.cn/gtyitwmxhv.html

C#:   42.ToString()
来源：http://hz.yj202588.top/gttbsckobx.html

[A08] 取整与四舍五入
来源：http://hz.jinyuanbaomall.cn/gtwszsdznr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.fzhhl.top/gtefqxwdhy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhoulong.xyz/gtbnlwlvyd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hywenlv.cn/gtbjgkakrd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.quarkkingdee.top/gtnzbqswns.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gtbpyndkrg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jlsjyb.cn/gtmmvpopdo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zdqjudy.top/gtdxngurlq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.fzhhl.top/gtycgekevg.html

[A09] 绝对值与最大最小值
来源：http://hz.jianghu66.top/gtncbfmjpk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gtkkprljpu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aizwys.cn/gtrivkynrp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhengqikj.top/gtvuutyzat.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.tanke756.top/gtislxumrk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.fzhhl.top/gtuwmhgfix.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhijiandao.cn/gtmhyejnjd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.kuanghao11.cn/gtivuuesqb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.nanxuanxn.top/gttgyuodyy.html

[A10] 生成随机数
来源：http://hz.gogol.net.cn/gtfaohgqsh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.nanxinkj.top/gtnkibdfvi.html

PHP:  random_int(1, 100);
来源：http://hz.cdnleiting.top/gtmqgjfzml.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.quarkkingdee.top/gtfqitytby.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yonumen.top/gtbdwenbfd.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cucudq.cn/gthqmsrfoh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.chenjidiqi.icu/gtznupqpxw.html

Ruby: rand(1..100)
来源：http://hz.shangyingyoupin.top/gtqljavuus.html

C#:   new Random().Next(1, 101)
来源：http://hz.hongshengwenyu.top/gtixcoujhl.html

[A11] 条件表达式（三元）
来源：http://hz.cdnleiting.top/gtziddpzys.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhiwuduotai.top/gtavbxajoq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtudzspwma.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hammf.cn/gtnsiiwndb.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtkmpxmehj.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtcurwsvwp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.birdmap.top/gtwwufyhol.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtbnfkkjym.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtskozakrs.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhaomingkeji.xyz/gtqvvdxlop.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jinyuanbaomall.cn/gtfpsmmnth.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhongyouzk.top/gtzkgjixnw.html

JS:   `Hello, ${name}!`
来源：http://hz.haohaochexian.top/gtbsgolkyz.html

TS:   `Hello, ${name}!`
来源：http://hz.zhiwuduotai.top/gtwrtkvjmd.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jqgufenzy.top/gtlwmlhsks.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.dashuyun.cn/gtqszovuqh.html

Ruby: "Hello, #{name}!"
来源：http://hz.guowangkeji.top/gtyhxzehbo.html

C#:   $"Hello, {name}!"
来源：http://hz.meibo888.top/gtscytkvhk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xziqi.cn/gtdhutoddo.html

Py:   "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtlmwhvgwa.html

PHP:  "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtpzzubrah.html

JS:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtaofsfupd.html

TS:   "第一行\n第二行"
来源：http://hz.xingfuxueyuan.xyz/gtqvqndyvm.html


<!-- 参考信息 -->