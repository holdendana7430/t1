代发 wailian999

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtsblxvhpv.html

composer require --dev phpstan/phpstan
来源：http://hz.9152youxi.cn/gtplclnivi.html

[U80] PHP：代码规范修复
来源：http://hz.yuxming.cn/gtxhbozzmr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jqgufenzy.top/gteanyhrco.html

[U81] JS：初始化项目
来源：http://hz.yj202588.top/gtwmevhtyt.html

npm init -y;  npm i express
来源：http://hz.mhx1999.top/gtxgbjgowi.html

[U82] JS：package.json 脚本
来源：http://hz.ydjk.org.cn/gtlsfaibwo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cdnleiting.top/gtekzuwhjo.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhijiandao.cn/gtuambrpwu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.andypj.xyz/gtlngoduxu.html

[U84] JS：CommonJS 写法
来源：http://hz.zhixingplan.top/gtbqwfnudb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtyveuvlsc.html

[U85] JS：可选链
来源：http://hz.kuanghao11.cn/gtktkopdbt.html

a?.b?.c
来源：http://hz.fengsongda.top/gtrjirisrf.html

[U86] JS：空值合并
来源：http://hz.cucudq.cn/gtrlcudlys.html

a ?? b
来源：http://hz.jinghuilouyu.cn/gtsqdsubbu.html

[U87] JS：解构默认值
来源：http://hz.wangdashe.top/gtcduvvuxt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.redwolf501.top/gtgqiyfnlv.html

[U88] JS：对象展开合并
来源：http://hz.jinqigfzy.top/gtsnzavhwn.html

{ ...a, ...b }
来源：http://hz.pycfn.com/gtjylzwyvt.html

[U89] JS：数组去重
来源：http://hz.jianghu66.top/gthojvdyzb.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtejnovjve.html

[U90] JS：数字数组排序
来源：http://hz.sweek.top/gtkpczohke.html

[...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtxyuzxngf.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtmymlpngw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tianlin.xyz/gtluchquxo.html

[U92] JS：深拷贝
来源：http://hz.bjfxy.top/gtgnqziroc.html

structuredClone(obj)
来源：http://hz.guowangkeji.top/gtdviqjzur.html

[U93] JS：模板字符串
来源：http://hz.zhixingplan.top/gtdehzhybt.html

`共 ${n} 条`
来源：http://hz.fzhhl.top/gtztndmjtw.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtpyjifbdf.html

const double = x => x * 2;
来源：http://hz.hfpthk.cn/gtcttzcxei.html

[U95] JS：Promise 包装
来源：http://hz.tianlin.xyz/gtsktqtxhh.html

new Promise((resolve, reject) => {})
来源：http://hz.chenzaomai.com/gtvpkonpta.html

[U96] JS：async/await 与异常
来源：http://hz.yangfankeji.com/gttltnlmpm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtgkklbgsn.html

[U97] JS：并发请求
来源：http://hz.xingfuxueyuan.xyz/gtwmbwaxcn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtfkvfwfmt.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenjidiqi.icu/gtbkotxxdb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gtivpqfzys.html

[U99] JS：事件监听
来源：http://hz.cucudq.cn/gtjewurkbn.html

el.addEventListener("click", e => {})
来源：http://hz.hammf.cn/gtdbfywaez.html

[U100] JS：DOM 查询
来源：http://hz.zhaomingkeji.xyz/gtsefgxwro.html

document.querySelector(".item")
来源：http://hz.iojbl.cn/gtysgtpwgo.html

[U101] JS：classList 操作
来源：http://hz.chenzaomai.com/gtbfdfnuct.html

el.classList.toggle("active")
来源：http://hz.cdnleiting.top/gttpqhxoif.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gtotoxjagg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnxiangtu.top/gtheezbmir.html

[U103] JS：定时器
来源：http://hz.ppjwa.cn/gtbgmltrbb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hnxiangtu.top/gtctqkogvu.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtfglogfkm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtkrkovkwj.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gtamdzapus.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sysykeji.top/gtffpidsxb.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtgyogooxx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtrszqsuli.html

[U107] JS：数字千分位
来源：http://hz.nanxinkj.top/gtngzkzndz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.bjfxy.top/gthfrxlgkn.html

[U108] JS：随机整数
来源：http://hz.hnxiangtu.top/gtjnfblbcl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hongshengwenyu.top/gtflhraidn.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gtrakzycsu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtyhehaisf.html

[U110] JS：数组分块
来源：http://hz.snrcjt.cn/gthhnpjodm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.snrcjt.cn/gtmhsokkxy.html

[U111] JS：对象转 Map
来源：http://hz.yj202588.top/gtttbgpomy.html

new Map(Object.entries(obj))
来源：http://hz.jlsjyb.cn/gtimjpandk.html

[U112] JS：字符串补位
来源：http://hz.chenzaomai.com/gtvtmzbnhn.html

"7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtthflnwgp.html

[U113] JS：正则替换全部
来源：http://hz.jlsjyb.cn/gtbfkhtboj.html

s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtdepgdzdc.html

[U114] JS：JSON 深比较
来源：http://hz.nwbrower.top/gtajcaxkrs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtmsevdvsu.html

[U115] JS：生成 UUID
来源：http://hz.pycfn.com/gtergywfdk.html

crypto.randomUUID()
来源：http://hz.daxiang520.top/gtafprukuf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jqgufenzy.top/gtxbcsiotf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pengpengdd.cyou/gthgsyvrgs.html

[U117] JS：单元测试
来源：http://hz.yongpay.top/gtmyybgiee.html

npm i -D vitest;  npx vitest
来源：http://hz.bjfxy.top/gtxzawsiqx.html

[U118] JS：开发服务器
来源：http://hz.redwolf501.top/gtfzakjzeg.html

npm i -D vite;  npx vite
来源：http://hz.jinyuanbaomall.cn/gthskbfvtb.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtkmoaswvf.html

npx vite build
来源：http://hz.jinqigfzy.top/gtvhoczcst.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuanzhike.top/gtxraoondj.html

import.meta.env.VITE_API_URL
来源：http://hz.fzhhl.top/gtcqzvtijm.html

================================================================================
来源：http://hz.gotoacloud.top/gtqcadkpkg.html

统计汇总
来源：http://hz.jinqigufen.top/gtlcwfrmpf.html

================================================================================
来源：http://hz.yvedp.cn/gtreuxaign.html

按语言统计（条）：
来源：http://hz.c1oappe.top/gtjbdpqisy.html

Python ......... 252
来源：http://hz.nwbrower.top/gtuinfsvtg.html

PHP ............ 252
来源：http://hz.vqdsnc.cn/gtjlbszsix.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gttzqxvqkq.html

TypeScript ..... 212
来源：http://hz.fzhhl.top/gtvlluhogw.html

Java ........... 212
来源：http://hz.quarkkingdee.top/gtnxckfotn.html

Go ............. 212
来源：http://hz.sweek.top/gtddadshxw.html

Ruby ........... 212
来源：http://hz.feifeiyinyue.top/gtflbbjokb.html

C# ............. 212
来源：http://hz.haohaochexian.top/gtzorfbgrm.html

C .............. 30
来源：http://hz.zycfv.cn/gtiqxmuftc.html

C++ ............ 30
来源：http://hz.aibaodan.cn/gttohamrvg.html

SQL ............ 90
来源：http://hz.tian-w.cn/gtkzeelnwd.html

Bash ........... 80
来源：http://hz.andypj.xyz/gteeflkrgc.html

Kotlin ......... 15
来源：http://hz.jyoumei.cn/gtqnpsixwn.html

Swift .......... 15
来源：http://hz.zdqjudy.top/gtglgduimz.html

Lua ............ 10
来源：http://hz.havefunace.top/gtssjumvvc.html

Perl ........... 10
来源：http://hz.9152youxi.cn/gtadpcwngl.html

Scala .......... 10
来源：http://hz.kuanghao11.cn/gtiljpgzgq.html

------------------------------------
来源：http://hz.zhengqikj.top/gtlgkgjxya.html

合计 ........... 2106 条
来源：http://hz.cucudq.cn/gtdqxdqxyw.html

按章节统计：
来源：http://hz.aizwys.cn/gtjqanzphg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.redwolf501.top/gtrkyhunqr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtlrxhlazk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gtwvvuqwxx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.meibo888.top/gtutcvsqoe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nanxuanxn.top/gtrcpftphb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtqwyhzgqe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtjdxvbhbx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtmsrpcrwp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtmuvlnqid.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.quarkkingdee.top/gtoqsqufhe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtwisbfuam.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtyumfkctq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtztfpwwuf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.havefunace.top/gtiqqfywyl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydzc1.top/gtepnfywsk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtdpbgivya.html

Q SQL 专题                              90
来源：http://hz.0kj1m.cn/gtontmkxpd.html

R Bash 专题                             80
来源：http://hz.yanxiufei.cn/gtgtupzsic.html

S C / C++ 专题                          60
来源：http://hz.chenlongwang.top/gtldxcaguh.html

T 其他语言补充                          60
来源：http://hz.kuanghao11.cn/gttkouhauj.html

U 高频实用片段                         120
来源：http://hz.sufxvd.cn/gtjgcbhqlf.html

------------------------------------
来源：http://hz.yuxming.cn/gtutimmbgp.html

合计                                  2106 条
来源：http://hz.shangyingyoupin.top/gtmompkpmk.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtqawznimm.html

使用提醒
来源：http://hz.zhengqikj.top/gtawgxzalm.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtgqcypbxe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj20258888.top/gtpxyjkczq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shanyushiyangkeji.top/gtrwktazqb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.quarkkingdee.top/gtpixdqspy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gogol.net.cn/gtshycbygi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.vqdsnc.cn/gtadjfnfdr.html

—— 文件结束 ——
来源：http://hz.pengpengdd.cyou/gtmhpwrkur.html

================================================================================
来源：http://hz.sysykeji.top/gtfmxzbktl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.haohaochexian.top/gtcibaiyea.html

Common Programming Examples Cheat Book
来源：http://hz.havefunace.top/gtumkzymjb.html

================================================================================
来源：http://hz.daria6918.cn/gtxvcedekg.html

【收录内容】
来源：http://hz.xziqi.cn/gtylijisfb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jqgfzy.top/gtnuamkrub.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fzhhl.top/gtxcmojygu.html

SQL · Bash · C · C++
来源：http://hz.zdqjudy.top/gtfwfetfxq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xinyue.icu/gtwzrgrogj.html

【使用说明】
来源：http://hz.guannengcc.top/gtyjguhgwm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ywan-chungtsiang.top/gtgtzwdvrg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nwbrower.top/gtxcahqoid.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.guannengcc.top/gtvbyxooux.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yongpay.top/gteyulwbzs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtmohpzhwp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.aizwys.cn/gtcfotfhlz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yongpay.top/gtmsnhczdy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hysaishi.cn/gtesaszyeh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yonumen.top/gtelglsagu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenzaomai.com/gtmqbbcqax.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.fengsongda.top/gtrmriclbo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgfzy.top/gtsnqfnoyd.html

【文件统计】
来源：http://hz.hfpthk.cn/gtdjxlnsrr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cashguo.top/gtyldnhgeo.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtdmuxefgp.html

目  录
来源：http://hz.sufxvd.cn/gtrmfukfga.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gttakwnsft.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.feifeiyinyue.top/gtjbsbnans.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtfeofoizn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtezglwxvj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtkrxhqark.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gtvidaoxgl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.meibo888.top/gtcyybiqdn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gthboacgaw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jiagoushi.top/gtyzoxrkvw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gttztawqfq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.fengsongda.top/gtcvdpjadj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtyomgamoy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtlteffzfh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtfpjqknun.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtdxpnrrfp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gttdywwinh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtpgivyyjv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.quarkkingdee.top/gtknfevpjv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtxmugcjnj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xuetiantiany.cn/gtwnvtkldt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtdxkaoscm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtlrwqhqwu.html

================================================================================
来源：http://hz.cdnleiting.top/gtsqytccjq.html

A. 基础语法与类型
来源：http://hz.shanyushiyangtech.top/gtauylxitf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtzboxzvhf.html

[A01] Hello World
来源：http://hz.yanxiufei.cn/gtnxjlrqxv.html

Py:   print("Hello, World!")
来源：http://hz.yangfankeji.com/gtarmmagbp.html

PHP:  echo "Hello, World!";
来源：http://hz.guowangkeji.top/gtzegghayz.html

JS:   console.log("Hello, World!");
来源：http://hz.zycfv.cn/gtzyboljzb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ydjk.org.cn/gtvdehvgvl.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtgnsvzofd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yonumen.top/gtsdxljztf.html

Ruby: puts "Hello, World!"
来源：http://hz.zhoulong.xyz/gtnbflsxzw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xinyue.icu/gtglwwuqkl.html

[A02] 变量声明与赋值
来源：http://hz.xuetiantiany.cn/gtvtxqmfqy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuetiantiany.cn/gtngbisasg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.mhx1999.top/gtnmcbwokl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtquvrhqsc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sxryk.cn/gtpxgoaoow.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.316326.xyz/gtbhpewqcc.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenjidiqi.icu/gtnnsdociy.html

Ruby: name = "Alex"; age = 20
来源：http://hz.9152youxi.cn/gtuwihrnad.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.tian-w.cn/gteqolznef.html

[A03] 常量定义
来源：http://hz.hysaishi.cn/gtgjxgdhxx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gotoacloud.top/gtsbrqznhk.html

PHP:  const PI = 3.14159;
来源：http://hz.hfpthk.cn/gtqpgpkstq.html

JS:   const PI = 3.14159;
来源：http://hz.smart0.xyz/gtsargmkhm.html

TS:   const PI: number = 3.14159;
来源：http://hz.iojbl.cn/gtjytswvwm.html

Java: static final double PI = 3.14159;
来源：http://hz.daxiang520.top/gtzorblrli.html

Go:   const PI = 3.14159
来源：http://hz.sweek.top/gtauhfygfk.html

Ruby: PI = 3.14159
来源：http://hz.yueranfly.top/gtiopherqf.html

C#:   const double PI = 3.14159;
来源：http://hz.tanke756.top/gtgucvrkhr.html

[A04] 判断变量类型
来源：http://hz.sxryk.cn/gteqlxjalk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.redwolf501.top/gtusjmdxyw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ppjwa.cn/gtywboulbm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangshuangyany.cn/gtwqvpaygk.html

TS:   typeof x; x instanceof Date
来源：http://hz.cucudq.cn/gtbutcndva.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shangyingyoupin.top/gtalryeuly.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xziqi.cn/gtvhldtycw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nwbrower.top/gtrpszvwzn.html

C#:   x.GetType().Name; x is int
来源：http://hz.9152youxi.cn/gtwvtyuyyn.html

[A05] 整数除法与取模
来源：http://hz.quarkkingdee.top/gtblsvkuwc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.andypj.xyz/gtfiksnsmm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yj202588.top/gtdycexohr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhijiandao.cn/gtlequkpxn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.c1oappe.top/gteettjxey.html

Java: 7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gtpwtulzyc.html

Go:   7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtutwzyvjj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtqqvtvpms.html

C#:   7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtadvhxpan.html

[A06] 字符串转数字
来源：http://hz.aizwys.cn/gtcqnxiuwq.html

Py:   int("42"); float("3.14")
来源：http://hz.jiagoushi.top/gttoilosjc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.sxryk.cn/gthzfozoyo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cashguo.top/gtnbnhbikc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cashguo.top/gtjwunllrs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yvedp.cn/gtepcphusm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.andypj.xyz/gtnlaixnpl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinyuanbaomall.cn/gtboombbis.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ybcxt.top/gtpalvzbqa.html

[A07] 数字转字符串
来源：http://hz.svipenyu.cn/gtqfkrlqtk.html

Py:   str(42)
来源：http://hz.snrcjt.cn/gtkjieprmy.html

PHP:  (string) 42; strval(42)
来源：http://hz.jianghu66.top/gtinlsavsi.html

JS:   String(42); (42).toString()
来源：http://hz.sufxvd.cn/gtjmicfcur.html

TS:   String(42)
来源：http://hz.snrcjt.cn/gtqjialynl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sweek.top/gtrwcetesi.html

Go:   strconv.Itoa(42)
来源：http://hz.quarkkingdee.top/gtosbkvtvh.html

Ruby: 42.to_s
来源：http://hz.yj202588.top/gtkompuylx.html

C#:   42.ToString()
来源：http://hz.zhengqikj.top/gtkirodriw.html

[A08] 取整与四舍五入
来源：http://hz.nwbrower.top/gtkzutsrza.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.sysykeji.top/gtpdmeowrc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tian-w.cn/gttfwogwdn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhiwuduotai.top/gtudqlljtj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xziqi.cn/gtjxpvkewt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtczznawzp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.dashuyun.cn/gtplrkpgtn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.snrcjt.cn/gtqiqenuyr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj202588.top/gtqivvwyha.html

[A09] 绝对值与最大最小值
来源：http://hz.cheryme.top/gttyuhjziu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhijiandao.cn/gteufhzfwz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinghuilouyu.cn/gtrboydaxw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.redwolf501.top/gtlqgmawoh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.wangshuangyany.cn/gtbomyvqjm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.feifeiyinyue.top/gtpuskfzwk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.vqdsnc.cn/gtegdtxkun.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tian-w.cn/gtiqfuxnmj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhixingplan.top/gtysewifyz.html

[A10] 生成随机数
来源：http://hz.shanyushiyangkeji.top/gtuwphidfd.html

Py:   import random; random.randint(1, 100)
来源：http://hz.shzxlz.cn/gtyveqgrxe.html

PHP:  random_int(1, 100);
来源：http://hz.chenjidiqi.icu/gttbefaqmb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.aibaodan.cn/gtviomribv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ywan-chungtsiang.top/gthuaxxado.html

Java: new Random().nextInt(100) + 1
来源：http://hz.sufxvd.cn/gtkxuaxfcd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yvedp.cn/gtrfrtjsyv.html

Ruby: rand(1..100)
来源：http://hz.jianghu66.top/gtulhcwbag.html

C#:   new Random().Next(1, 101)
来源：http://hz.zycfv.cn/gtamuupkyx.html

[A11] 条件表达式（三元）
来源：http://hz.yangfankeji.com/gtrvqhdvbn.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.tianlin.xyz/gtdtsgzghu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtoeuzfivh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtkpbobvlz.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtstmbgvlx.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtivmrqcna.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xuetiantiany.cn/gtgljfubiq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hnxiangtu.top/gtaybjvcnf.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtigcqcgxh.html

[A12] 字符串插值 / 格式化
来源：http://hz.guowangkeji.top/gtnyrgfuuy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yanxiufei.cn/gtwtnkvbgd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yuanzhike.top/gtafwzriay.html

JS:   `Hello, ${name}!`
来源：http://hz.gaohongyu789.top/gtjjwbwfbl.html

TS:   `Hello, ${name}!`
来源：http://hz.yj20258888.top/gtrrwnapol.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.52xcode.cn/gtqfrllnoh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.tianlin.xyz/gtbywbhiau.html

Ruby: "Hello, #{name}!"
来源：http://hz.daxiang520.top/gtabiymebx.html

C#:   $"Hello, {name}!"
来源：http://hz.0kj1m.cn/gtbchjnvbr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xuetiantiany.cn/gtywtfbfwu.html


<!-- 参考信息 -->