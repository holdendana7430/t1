代发 wailian999

[U77] PHP：模板渲染
来源：http://hz.jinghuilouyu.cn/gtzcbkdpvb.html

composer require twig/twig
来源：http://hz.daxiang520.top/gtojiifgzs.html

[U78] PHP：单元测试
来源：http://hz.pycfn.com/gtizfyctha.html

composer require --dev phpunit/phpunit
来源：http://hz.wangshuangyany.cn/gtwdklmtgu.html

[U79] PHP：静态分析
来源：http://hz.9152youxi.cn/gtvirdqbsq.html

composer require --dev phpstan/phpstan
来源：http://hz.jinqigufen.top/gtzcuiwale.html

[U80] PHP：代码规范修复
来源：http://hz.xziqi.cn/gtwyarjbsq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxinkj.top/gtzehgqmnd.html

[U81] JS：初始化项目
来源：http://hz.zhijiandao.cn/gtjbitkmmv.html

npm init -y;  npm i express
来源：http://hz.zdqjudy.top/gtgpbleqrh.html

[U82] JS：package.json 脚本
来源：http://hz.daxiang520.top/gtqxkyxeku.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shangyingyoupin.top/gtjquwsiev.html

[U83] JS：ES Module 导入导出
来源：http://hz.0kj1m.cn/gtrxhurbcw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gogol.net.cn/gtnebjhraf.html

[U84] JS：CommonJS 写法
来源：http://hz.jqgfzy.top/gtbdnpasov.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dashuyun.cn/gtrnkxayxx.html

[U85] JS：可选链
来源：http://hz.chenlongwang.top/gtypibjsku.html

a?.b?.c
来源：http://hz.sweek.top/gtjmzdorcv.html

[U86] JS：空值合并
来源：http://hz.daria6918.cn/gtfkrubpla.html

a ?? b
来源：http://hz.shanyushiyangtech.top/gtcnmtnhbs.html

[U87] JS：解构默认值
来源：http://hz.shuidangran.top/gtcrjorupj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xylfe.cn/gthndwspkm.html

[U88] JS：对象展开合并
来源：http://hz.xingfuxueyuan.xyz/gtdpkkqpnf.html

{ ...a, ...b }
来源：http://hz.wangshuangyany.cn/gtunhpahgd.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gtvgactcth.html

[...new Set(arr)]
来源：http://hz.xziqi.cn/gtqowpsyuv.html

[U90] JS：数字数组排序
来源：http://hz.chenjidiqi.icu/gtaksaevbn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtjvmhnsis.html

[U91] JS：对象键值遍历
来源：http://hz.haohaochexian.top/gtuizskjab.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.redwolf501.top/gtygmyhpfi.html

[U92] JS：深拷贝
来源：http://hz.hnxiangtu.top/gtforbcfzw.html

structuredClone(obj)
来源：http://hz.tanke756.top/gtmedifirq.html

[U93] JS：模板字符串
来源：http://hz.cashguo.top/gttjkoogcr.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtmcjskzdz.html

[U94] JS：箭头函数
来源：http://hz.tanke756.top/gtrpvjtjmm.html

const double = x => x * 2;
来源：http://hz.quarkkingdee.top/gtmxhoqavy.html

[U95] JS：Promise 包装
来源：http://hz.dianchejie.cn/gtoujydgxn.html

new Promise((resolve, reject) => {})
来源：http://hz.ehwqpu.com/gtdtxaxhfv.html

[U96] JS：async/await 与异常
来源：http://hz.xziqi.cn/gtsqsrfpbe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtcniomces.html

[U97] JS：并发请求
来源：http://hz.shangyingyoupin.top/gtcnlvoocx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gttwlcpche.html

[U98] JS：fetch 带 JSON
来源：http://hz.ybcxt.top/gtgauxxnww.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtrakuxfui.html

[U99] JS：事件监听
来源：http://hz.daxiang520.top/gtbcykpuoj.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtosqllgec.html

[U100] JS：DOM 查询
来源：http://hz.xinyue.icu/gtwgnhseqe.html

document.querySelector(".item")
来源：http://hz.chenlongwang.top/gtbrjgzros.html

[U101] JS：classList 操作
来源：http://hz.xingfuxueyuan.xyz/gtkwlcegvm.html

el.classList.toggle("active")
来源：http://hz.xuetiantiany.cn/gtkyrfzizj.html

[U102] JS：本地存储
来源：http://hz.sufxvd.cn/gtscjgccua.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtqxhebxqd.html

[U103] JS：定时器
来源：http://hz.redwolf501.top/gtimbmyrpk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xziqi.cn/gtfjimoltx.html

[U104] JS：防抖
来源：http://hz.jinyuanbaomall.cn/gtvvxfymyf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtxibpgidt.html

[U105] JS：节流
来源：http://hz.zhengqikj.top/gtqgdtovxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gtizdgparn.html

[U106] JS：日期格式化
来源：http://hz.wangdashe.top/gtpwvanspp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zycfv.cn/gtmxhlulcg.html

[U107] JS：数字千分位
来源：http://hz.hongshengwenyu.top/gtnfnrzzij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tian-w.cn/gtxnztopuy.html

[U108] JS：随机整数
来源：http://hz.xylfe.cn/gtrulyvccz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cdnleiting.top/gtemcfprdc.html

[U109] JS：数组分组
来源：http://hz.quarkkingdee.top/gtrlqsispn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gthufiieig.html

[U110] JS：数组分块
来源：http://hz.fengsongda.top/gttewrjyae.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nwbrower.top/gtnaiyycyx.html

[U111] JS：对象转 Map
来源：http://hz.smart0.xyz/gtfkenuwhr.html

new Map(Object.entries(obj))
来源：http://hz.c1oappe.top/gtaknipyfd.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtfmsrmryw.html

"7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtkqbjmkyu.html

[U113] JS：正则替换全部
来源：http://hz.yuanzhike.top/gthafoxfsa.html

s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtkgfivelw.html

[U114] JS：JSON 深比较
来源：http://hz.tianlin.xyz/gtozxjqkmo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtykrwbrnz.html

[U115] JS：生成 UUID
来源：http://hz.jinqigfzy.top/gttbhngvpa.html

crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtqvfrdljr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinghuilouyu.cn/gtwdmnowpj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinyuanbaomall.cn/gteufnvbog.html

[U117] JS：单元测试
来源：http://hz.yvedp.cn/gtalvldkas.html

npm i -D vitest;  npx vitest
来源：http://hz.zhongyouzk.top/gtrokfpkrv.html

[U118] JS：开发服务器
来源：http://hz.yanxiufei.cn/gtgqxgnqvc.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtrtqqxuty.html

[U119] JS：生产构建
来源：http://hz.0kj1m.cn/gtuzvuwsnt.html

npx vite build
来源：http://hz.daxiang520.top/gtecqnpfys.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gthyfpvkyc.html

import.meta.env.VITE_API_URL
来源：http://hz.yangfankeji.com/gteuwdqhdk.html

================================================================================
来源：http://hz.haohaochexian.top/gtcpsyzpap.html

统计汇总
来源：http://hz.xingfuxueyuan.xyz/gtaovzrkip.html

================================================================================
来源：http://hz.aizwys.cn/gttxnektwh.html

按语言统计（条）：
来源：http://hz.sweek.top/gtrjjjdinb.html

Python ......... 252
来源：http://hz.vqdsnc.cn/gtmgpzqdxy.html

PHP ............ 252
来源：http://hz.jqgfzy.top/gtlqxbztoa.html

JavaScript ..... 252
来源：http://hz.yuxming.cn/gtapvepyuh.html

TypeScript ..... 212
来源：http://hz.shzxlz.cn/gtkfbvjcvs.html

Java ........... 212
来源：http://hz.jinyuanbaomall.cn/gtxozcsgcz.html

Go ............. 212
来源：http://hz.daria6918.cn/gthwcjydwx.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtawpbzxod.html

C# ............. 212
来源：http://hz.wangshuangyany.cn/gtgvmbymua.html

C .............. 30
来源：http://hz.pycfn.com/gtqqqttfbw.html

C++ ............ 30
来源：http://hz.jlsjyb.cn/gtzikblspy.html

SQL ............ 90
来源：http://hz.0kj1m.cn/gtiumqlwyn.html

Bash ........... 80
来源：http://hz.bjfxy.top/gtcvtkbmkv.html

Kotlin ......... 15
来源：http://hz.birdmap.top/gtgkjxljbb.html

Swift .......... 15
来源：http://hz.xuanzx.com/gtfuxxzxij.html

Lua ............ 10
来源：http://hz.jinqigufen.top/gtypbcymxz.html

Perl ........... 10
来源：http://hz.ydjk.org.cn/gtyfsuuytb.html

Scala .......... 10
来源：http://hz.cqqwz.cn/gttweqeasj.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtsgbegnpl.html

合计 ........... 2106 条
来源：http://hz.yueranfly.top/gtqswnevpx.html

按章节统计：
来源：http://hz.svipenyu.cn/gtciaflzbl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jianghu66.top/gtvwjqibkb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtjdwrwiej.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtjsyxfjyj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtucakfkre.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jlsjyb.cn/gtsrkcobkx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gtoaavvlve.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtamwremxv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gtxwwsnlxc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtoqzpgekl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtjwlrbvdb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtckvwrdzs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtfozktwaj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtjpgcokzy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtmnocyjko.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangkeji.top/gtpzdxashn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtzbvicbjm.html

Q SQL 专题                              90
来源：http://hz.sxryk.cn/gtohliktiv.html

R Bash 专题                             80
来源：http://hz.cdnleiting.top/gthadjyvip.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtprklstpy.html

T 其他语言补充                          60
来源：http://hz.jqgfzy.top/gtgloqestw.html

U 高频实用片段                         120
来源：http://hz.cdnleiting.top/gtsrbcxzzf.html

------------------------------------
来源：http://hz.meibo888.top/gtmtdvbxuc.html

合计                                  2106 条
来源：http://hz.gzhubu.top/gtzyjytomw.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtjohcpxyr.html

使用提醒
来源：http://hz.ehwqpu.com/gtrmvzikfp.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtwerklibi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.0kj1m.cn/gtfkfdunhv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cashguo.top/gttdsoghiw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.birdmap.top/gticzltweo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gogol.net.cn/gtlcopbkgh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yongpay.top/gtcvlyfdzz.html

—— 文件结束 ——
来源：http://hz.smart0.xyz/gtmjlylkoy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtehnsbjdi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yanxiufei.cn/gtwzixmqwm.html

Common Programming Examples Cheat Book
来源：http://hz.cdnleiting.top/gtkewmziwb.html

================================================================================
来源：http://hz.fzhhl.top/gtajecikdg.html

【收录内容】
来源：http://hz.9152youxi.cn/gtvrrbtpxj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dashuyun.cn/gtiqmbjksp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhixingplan.top/gterrjqqsq.html

SQL · Bash · C · C++
来源：http://hz.cucudq.cn/gtyrdpvatp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dianchejie.cn/gtouyilvdh.html

【使用说明】
来源：http://hz.gzhubu.top/gtdznsdcsz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cqqwz.cn/gtugzszggn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258.top/gtmcmdxysn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.redwolf501.top/gtcowbesjy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pycfn.com/gtiviiltma.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ivvv.top/gtnumoswoa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shzxlz.cn/gtypnqxkkv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ydjk.org.cn/gtgvudbuog.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ehwqpu.com/gtnkzwqwdd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtfjrpbalh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tanke756.top/gtbvmoroke.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pycfn.com/gtpzhdnnrr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sweek.top/gtjmfgnrhl.html

【文件统计】
来源：http://hz.aibaodan.cn/gtmhjyvebx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtwqjairvq.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtwugmxupg.html

目  录
来源：http://hz.shanyushiyangtech.top/gtaudiqslz.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtkakvacvu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pengpengdd.cyou/gtbxjazccy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ywan-chungtsiang.top/gtjvbprohj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtggqkdwfw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gtliubpnoz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nwbrower.top/gtkthdghnl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.9152youxi.cn/gtllcngruo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtvbdybqtc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtkktmjghn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtmbxvtidy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.fzhhl.top/gtstnpwgwg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtidmsnwdb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtbbftpbqh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtysiifssw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtykhxpvjw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dianchejie.cn/gtupihbowe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtyxyyrvyu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydzc1.top/gtbfctluts.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinghuilouyu.cn/gtcmdgxfhb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shanyushiyangkeji.top/gtbgdyhonz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtshmivksg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hywenlv.cn/gtzlcygzeo.html

================================================================================
来源：http://hz.shzxlz.cn/gtigdtrzvi.html

A. 基础语法与类型
来源：http://hz.ybcxt.top/gtlmbmoxjl.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgpnlnikh.html

[A01] Hello World
来源：http://hz.yj202588.top/gtaxmvcoir.html

Py:   print("Hello, World!")
来源：http://hz.dashuyun.cn/gtwdingkna.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtgbecjffw.html

JS:   console.log("Hello, World!");
来源：http://hz.shuidangran.top/gthmozsyvl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhongyouzk.top/gtloblhrbx.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtkanukidq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jianghu66.top/gtynktpbfm.html

Ruby: puts "Hello, World!"
来源：http://hz.xziqi.cn/gtegnzogja.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.aizwys.cn/gtdnckjjlo.html

[A02] 变量声明与赋值
来源：http://hz.hnxiangtu.top/gticyvdilh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.daria6918.cn/gtuznqmgot.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.kuanghao11.cn/gtmawesiip.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cheryme.top/gtjuguvxrj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xinyue.icu/gtkyzgpcye.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zycfv.cn/gtmuahvcjf.html

Go:   name := "Alex"; age := 20
来源：http://hz.yuanzhike.top/gteufhoojs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.meibo888.top/gthmqsyvjt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ybcxt.top/gtllhtrvxd.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gtuafjankm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.9152youxi.cn/gtnhqelwip.html

PHP:  const PI = 3.14159;
来源：http://hz.daxiang520.top/gttdupfdrn.html

JS:   const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtqjdvneke.html

TS:   const PI: number = 3.14159;
来源：http://hz.daxiang520.top/gtalepglzr.html

Java: static final double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtecsgeiaq.html

Go:   const PI = 3.14159
来源：http://hz.cdnleiting.top/gtkttfezjy.html

Ruby: PI = 3.14159
来源：http://hz.gotoacloud.top/gtpibrnsmz.html

C#:   const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtrqtmpjan.html

[A04] 判断变量类型
来源：http://hz.jianghu66.top/gtirlatezk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.tanke756.top/gtdktzpysi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daria6918.cn/gtjzzwaica.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shzxlz.cn/gtjqdnubmx.html

TS:   typeof x; x instanceof Date
来源：http://hz.iojbl.cn/gthbczjpyt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yuxming.cn/gtbqafemfn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cucudq.cn/gtrukqnaht.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.pycfn.com/gtacmmtlis.html

C#:   x.GetType().Name; x is int
来源：http://hz.ybcxt.top/gtxyssiyru.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangtech.top/gtuntajsif.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hnxiangtu.top/gtaajtmasd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtnzfbevyf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.bjfxy.top/gtcvuacdmx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sweek.top/gtstttnwsw.html

Java: 7 / 2; 7 % 2
来源：http://hz.meibo888.top/gtegijypuv.html

Go:   7 / 2; 7 % 2
来源：http://hz.nanxuanxn.top/gtbqmugkqu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.c1oappe.top/gtewmxscnv.html

C#:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtmtijubmf.html

[A06] 字符串转数字
来源：http://hz.hysaishi.cn/gttpoqquts.html

Py:   int("42"); float("3.14")
来源：http://hz.gaohongyu789.top/gtrekjvqgp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hywenlv.cn/gtqkeivooc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.bjfxy.top/gtfkctedzs.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jianghu66.top/gthcqkmyvp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.daria6918.cn/gtdewcxhsn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.dianchejie.cn/gtjzlmxxtg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.52xcode.cn/gtnvbeuiqq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhiwuduotai.top/gtmrusiupl.html

[A07] 数字转字符串
来源：http://hz.yuxming.cn/gtngwwipnb.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtmkswuzdz.html

PHP:  (string) 42; strval(42)
来源：http://hz.9152youxi.cn/gtojkfnyyk.html

JS:   String(42); (42).toString()
来源：http://hz.tanke756.top/gtgcgfrhnu.html

TS:   String(42)
来源：http://hz.wangdashe.top/gtvtpmvtbi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nwbrower.top/gtysujprnp.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtwnimpnmq.html

Ruby: 42.to_s
来源：http://hz.mhx1999.top/gtmrlrivdr.html

C#:   42.ToString()
来源：http://hz.yj20258.top/gthsuecqjc.html

[A08] 取整与四舍五入
来源：http://hz.zhengqikj.top/gtsqxyshuq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.guannengcc.top/gtxwshiwyn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.nwbrower.top/gttqdoqfgg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jqgfzy.top/gtviwkvosj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.ydjk.org.cn/gtocbkhyad.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.smart0.xyz/gtpyfyfbqc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.9152youxi.cn/gtaneyjlnd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jyoumei.cn/gtyofaywmr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jianghu66.top/gtprtqibhz.html

[A09] 绝对值与最大最小值
来源：http://hz.ydjk.org.cn/gthrtprbmv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258.top/gtwikeokbl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinqigfzy.top/gtdbedkalr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.c1oappe.top/gtbpasydfz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cucudq.cn/gtzxzjcbmq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sysykeji.top/gtwfnonvsm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hysaishi.cn/gtohtxnliz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.aizwys.cn/gtdqjyfesz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.mhx1999.top/gtfcwgsbvy.html

[A10] 生成随机数
来源：http://hz.0kj1m.cn/gtvhjtbhww.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hfpthk.cn/gtkzkxrmdv.html

PHP:  random_int(1, 100);
来源：http://hz.hammf.cn/gtgmfkflyr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.pycfn.com/gtlrjgrdqv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xuetiantiany.cn/gtzerhrmqx.html

Java: new Random().nextInt(100) + 1
来源：http://hz.chenzaomai.com/gtzvdwkbmt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.gaohongyu789.top/gtmnuwxeqm.html

Ruby: rand(1..100)
来源：http://hz.jyoumei.cn/gtennqzmic.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhengqikj.top/gtddhlrzcj.html

[A11] 条件表达式（三元）
来源：http://hz.pengpengdd.cyou/gteqmsyedd.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.0kj1m.cn/gtymqitghi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtaumuclaq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtngiwdbry.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtskyketdw.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.hywenlv.cn/gtubvorttk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ivvv.top/gtbadlbvdo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.kuanghao11.cn/gtgavuywtx.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yuanzhike.top/gtvcgdxcsl.html

[A12] 字符串插值 / 格式化
来源：http://hz.jlsjyb.cn/gtnacfosil.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jyoumei.cn/gtvsvlloqr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sxryk.cn/gtdshqwrxl.html

JS:   `Hello, ${name}!`
来源：http://hz.hysaishi.cn/gtyhizfrxv.html

TS:   `Hello, ${name}!`
来源：http://hz.tianlin.xyz/gttwcdodkt.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhaomingkeji.xyz/gtozsnlbkb.html


<!-- 参考信息 -->