代发 wailian999

[U77] PHP：模板渲染
来源：http://hz.jlsjyb.cn/gtcohmixva.html

composer require twig/twig
来源：http://hz.ywan-chungtsiang.top/gteiwbqvii.html

[U78] PHP：单元测试
来源：http://hz.hysaishi.cn/gttizyxhsv.html

composer require --dev phpunit/phpunit
来源：http://hz.nwbrower.top/gtgtfuvhgk.html

[U79] PHP：静态分析
来源：http://hz.jyoumei.cn/gtwrspuzuc.html

composer require --dev phpstan/phpstan
来源：http://hz.tian-w.cn/gtsqcwqhst.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtengnmaii.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ehwqpu.com/gtsusycyvt.html

[U81] JS：初始化项目
来源：http://hz.tian-w.cn/gtfxlimdww.html

npm init -y;  npm i express
来源：http://hz.ehwqpu.com/gtngdjiovk.html

[U82] JS：package.json 脚本
来源：http://hz.yj20258.top/gtdnlgzqft.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xylfe.cn/gtlqklcnpi.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydjk.org.cn/gtqtanxkce.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sweek.top/gtkbfjvyhn.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtxikmlfok.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ydjk.org.cn/gtyxauypqp.html

[U85] JS：可选链
来源：http://hz.hammf.cn/gtxxxmdkpn.html

a?.b?.c
来源：http://hz.kuanghao11.cn/gtyinxoius.html

[U86] JS：空值合并
来源：http://hz.vqdsnc.cn/gtctnjlcyc.html

a ?? b
来源：http://hz.cqqwz.cn/gtnwobebno.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gteyeifzgf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhixingplan.top/gtrcfosdtj.html

[U88] JS：对象展开合并
来源：http://hz.bjfxy.top/gtvhzyazce.html

{ ...a, ...b }
来源：http://hz.jinqigfzy.top/gtcdccqows.html

[U89] JS：数组去重
来源：http://hz.haohaochexian.top/gtaovwbrsw.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtludcgwmr.html

[U90] JS：数字数组排序
来源：http://hz.daria6918.cn/gtafapuhfc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtlnqxffqy.html

[U91] JS：对象键值遍历
来源：http://hz.feifeiyinyue.top/gtxqofgndb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258888.top/gtbrbxijcr.html

[U92] JS：深拷贝
来源：http://hz.ydzc1.top/gtplciinbh.html

structuredClone(obj)
来源：http://hz.svipenyu.cn/gttzbchuci.html

[U93] JS：模板字符串
来源：http://hz.yj20258888.top/gtnlfomfqt.html

`共 ${n} 条`
来源：http://hz.quarkkingdee.top/gtdpfnytnn.html

[U94] JS：箭头函数
来源：http://hz.jianghu66.top/gtnkqpqfjd.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gteqixnmvk.html

[U95] JS：Promise 包装
来源：http://hz.gogol.net.cn/gtxwocpycs.html

new Promise((resolve, reject) => {})
来源：http://hz.zhoulong.xyz/gtsxlorjib.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtkawvtckf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtpdqthhng.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtgwompwoi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtcodxruuw.html

[U98] JS：fetch 带 JSON
来源：http://hz.yvedp.cn/gtckcxkqjy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daria6918.cn/gtnhtxpbkg.html

[U99] JS：事件监听
来源：http://hz.yangfankeji.com/gteviknedd.html

el.addEventListener("click", e => {})
来源：http://hz.cheryme.top/gtbwmzqcce.html

[U100] JS：DOM 查询
来源：http://hz.nanxuanxn.top/gtfbinafpe.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtwlnlxtic.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtehkeofvv.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gtrdtzzvwk.html

[U102] JS：本地存储
来源：http://hz.fengsongda.top/gtuefpzmoi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hammf.cn/gttnmgoebz.html

[U103] JS：定时器
来源：http://hz.andypj.xyz/gtykisejvk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhixingplan.top/gtotxpjpjy.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtzgxbbbey.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gttccedxuu.html

[U105] JS：节流
来源：http://hz.52xcode.cn/gtoatbmeaf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ehwqpu.com/gtsiqcviji.html

[U106] JS：日期格式化
来源：http://hz.chenjidiqi.icu/gtlwnvuypd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.chenlongwang.top/gtzfcpjvfn.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtjmxroild.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gaohongyu789.top/gtbiwvcppr.html

[U108] JS：随机整数
来源：http://hz.hysaishi.cn/gtxyovauwb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.smart0.xyz/gtjdmbgwvm.html

[U109] JS：数组分组
来源：http://hz.snrcjt.cn/gtminqzpar.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtugexqhzt.html

[U110] JS：数组分块
来源：http://hz.hysaishi.cn/gtzyxurrff.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.0kj1m.cn/gtmladialj.html

[U111] JS：对象转 Map
来源：http://hz.aibaodan.cn/gttgfhmlmp.html

new Map(Object.entries(obj))
来源：http://hz.sufxvd.cn/gtfortjmmz.html

[U112] JS：字符串补位
来源：http://hz.jinghuilouyu.cn/gtrlomqzdb.html

"7".padStart(3, "0")
来源：http://hz.birdmap.top/gtiwehozyp.html

[U113] JS：正则替换全部
来源：http://hz.tian-w.cn/gtffmluwgg.html

s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gttancirhp.html

[U114] JS：JSON 深比较
来源：http://hz.pycfn.com/gtlhcgckgr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtitcdvzvp.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtidhqgvrp.html

crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtcgubfjmn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangshuangyany.cn/gtefxsxsxc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.quarkkingdee.top/gtkulmntze.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtnzrltwhk.html

npm i -D vitest;  npx vitest
来源：http://hz.tian-w.cn/gtyvxcfhem.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gtxxmuqgiz.html

npm i -D vite;  npx vite
来源：http://hz.iojbl.cn/gtjvntmzqt.html

[U119] JS：生产构建
来源：http://hz.hnxiangtu.top/gtxpgjwbyt.html

npx vite build
来源：http://hz.daria6918.cn/gtvkwtxmac.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuetiantiany.cn/gtouvyxcoe.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtmsksfmlf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvjxwclzj.html

统计汇总
来源：http://hz.chenlongwang.top/gtccmtuyqu.html

================================================================================
来源：http://hz.vqdsnc.cn/gttdagjcxa.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gthwowtdpi.html

Python ......... 252
来源：http://hz.xylfe.cn/gtlniactbz.html

PHP ............ 252
来源：http://hz.redwolf501.top/gthjdyiknb.html

JavaScript ..... 252
来源：http://hz.pycfn.com/gtoxiiswgl.html

TypeScript ..... 212
来源：http://hz.shzxlz.cn/gtprfsrsok.html

Java ........... 212
来源：http://hz.bjfxy.top/gtbdcqasmn.html

Go ............. 212
来源：http://hz.zhengqikj.top/gtgibfijql.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gtsykrmgdp.html

C# ............. 212
来源：http://hz.jqgufenzy.top/gtvkfnxcnq.html

C .............. 30
来源：http://hz.zhixingplan.top/gtiqmgwurp.html

C++ ............ 30
来源：http://hz.havefunace.top/gtmrvncxse.html

SQL ............ 90
来源：http://hz.feifeiyinyue.top/gtcgqkvzrl.html

Bash ........... 80
来源：http://hz.yangfankeji.com/gtlzwubadu.html

Kotlin ......... 15
来源：http://hz.zhongyouzk.top/gtqjspmncp.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtklyemigg.html

Lua ............ 10
来源：http://hz.shuidangran.top/gthgxmbctb.html

Perl ........... 10
来源：http://hz.sweek.top/gtklevxyfi.html

Scala .......... 10
来源：http://hz.meibo888.top/gtunqsvmpw.html

------------------------------------
来源：http://hz.aizwys.cn/gtusqzcidn.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtzaoikmqm.html

按章节统计：
来源：http://hz.sysykeji.top/gtgojkqwnl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtoyzwxkdx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtroqaqzik.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtgrwgruew.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jianghu66.top/gtsajoyiwh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gtqvcjvmgx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtgrzesnrf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtzpmaamsc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtvlzxlfev.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtiagxpube.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuxming.cn/gtxionspjg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtqnweiqbj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtfwvxfxqx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtweyeygmp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtvnqjjomz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.redwolf501.top/gtjlsjwqfq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtkamlskhe.html

Q SQL 专题                              90
来源：http://hz.kuanghao11.cn/gtongbxoth.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gtyaqcpzbn.html

S C / C++ 专题                          60
来源：http://hz.cucudq.cn/gtbpkouacy.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gtdrgrnndr.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtkjxkwnou.html

------------------------------------
来源：http://hz.yj20258.top/gttxpmwdnd.html

合计                                  2106 条
来源：http://hz.yanxiufei.cn/gtlznvfmdd.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtwpljbujb.html

使用提醒
来源：http://hz.hammf.cn/gtlmfnzfgd.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtrqqfzxkp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.pengpengdd.cyou/gtskwmbyiw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.vqdsnc.cn/gtptpwwpie.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtfdrhrvag.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cdnleiting.top/gtvvvuwqas.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hywenlv.cn/gtuayopove.html

—— 文件结束 ——
来源：http://hz.sxryk.cn/gtzjsiidmz.html

================================================================================
来源：http://hz.jinqigufen.top/gtyrozacix.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtbksmexro.html

Common Programming Examples Cheat Book
来源：http://hz.shzxlz.cn/gtwlffhhct.html

================================================================================
来源：http://hz.jyoumei.cn/gtqvsqlpxa.html

【收录内容】
来源：http://hz.guowangkeji.top/gtpcwcfhpf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dianchejie.cn/gtrsjkqmgq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj202588.top/gtegaepkpk.html

SQL · Bash · C · C++
来源：http://hz.dashuyun.cn/gtftzvhcfs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gotoacloud.top/gtsenitwyz.html

【使用说明】
来源：http://hz.zhoulong.xyz/gtrhitdqgz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shanyushiyangtech.top/gtuspvbwce.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jiagoushi.top/gtbaeyqllk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.mhx1999.top/gtbxtjpxbt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hammf.cn/gtlxiiyuni.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigfzy.top/gtzrlfjrph.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydjk.org.cn/gtczwciaxr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ehwqpu.com/gthzlqiogq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtymndware.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.iojbl.cn/gtlrrbabwu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gthhjvmbfb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gotoacloud.top/gtccjdvalb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hammf.cn/gtabaszwxv.html

【文件统计】
来源：http://hz.ivvv.top/gtwxldnbkh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ivvv.top/gtxhdnechl.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtvtkokrlp.html

目  录
来源：http://hz.jqgufenzy.top/gtemvnnrtk.html

--------------------------------------------------------------------------------
来源：http://hz.iojbl.cn/gtliatnbbf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtramyqlml.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtewzlvqjf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtddolnkdm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhengqikj.top/gtghxwunpl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.gaohongyu789.top/gtwngykdch.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtasvwljpl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtonhqbnqg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtwvsqvldt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gthddektjq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgfzy.top/gtfxgaasnr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gttxulqhcg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtarsgmonb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtbytzyrrc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shanyushiyangtech.top/gtulbbffsg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.feifeiyinyue.top/gtmpqdcrag.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtnmctvebc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydzc1.top/gtsdpphlee.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fengsongda.top/gtqrrkswlk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgufenzy.top/gtuejushqp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtktzdoffp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gthxryjbne.html

================================================================================
来源：http://hz.sweek.top/gtmavyoxhz.html

A. 基础语法与类型
来源：http://hz.cqqwz.cn/gtgvulpaqf.html

================================================================================
来源：http://hz.yonumen.top/gtdwqrcvua.html

[A01] Hello World
来源：http://hz.jiagoushi.top/gtwihvkwor.html

Py:   print("Hello, World!")
来源：http://hz.jqgfzy.top/gteaeslqms.html

PHP:  echo "Hello, World!";
来源：http://hz.tian-w.cn/gtfqirezsc.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtzmuocrlu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xuetiantiany.cn/gtvuveowkn.html

Java: System.out.println("Hello, World!");
来源：http://hz.bjfxy.top/gtofsjomvp.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtigpvztck.html

Ruby: puts "Hello, World!"
来源：http://hz.cucudq.cn/gtmsqpizfr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jianghu66.top/gtmrlwxknr.html

[A02] 变量声明与赋值
来源：http://hz.yvedp.cn/gtcqgdcrbc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinyuanbaomall.cn/gtguovmkli.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sufxvd.cn/gtrkngvavf.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hammf.cn/gtgrzrbigc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.andypj.xyz/gtziaimphy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ehwqpu.com/gtsdwmbsfr.html

Go:   name := "Alex"; age := 20
来源：http://hz.redwolf501.top/gtfekchcel.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ppjwa.cn/gtluqssluk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtwdfvewyo.html

[A03] 常量定义
来源：http://hz.vqdsnc.cn/gtpbrwnwrg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jqgfzy.top/gtnfssuzqb.html

PHP:  const PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtctiuhedw.html

JS:   const PI = 3.14159;
来源：http://hz.snrcjt.cn/gtssalmvhp.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtudvslutx.html

Java: static final double PI = 3.14159;
来源：http://hz.wangdashe.top/gtjlqgczbg.html

Go:   const PI = 3.14159
来源：http://hz.gzhubu.top/gtiynnzdcr.html

Ruby: PI = 3.14159
来源：http://hz.xuanzx.com/gtdoelcyka.html

C#:   const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtibdzriwz.html

[A04] 判断变量类型
来源：http://hz.jyoumei.cn/gtunixuxyq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xuetiantiany.cn/gtsdhxpfzq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.quarkkingdee.top/gttwvzejkj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yj20258888.top/gtygizdolp.html

TS:   typeof x; x instanceof Date
来源：http://hz.nanxinkj.top/gtcxvaehlf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gzhubu.top/gtkjmjdpoj.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.316326.xyz/gtkvufxelx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jinghuilouyu.cn/gtaoxigecf.html

C#:   x.GetType().Name; x is int
来源：http://hz.ppjwa.cn/gtbhfdzitu.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangtech.top/gtlrkkyqok.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.kuanghao11.cn/gtionpmvbz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jianghu66.top/gtsxvyioyt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtqkofoerd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hfpthk.cn/gthomyamjd.html

Java: 7 / 2; 7 % 2
来源：http://hz.316326.xyz/gtpainvmup.html

Go:   7 / 2; 7 % 2
来源：http://hz.kuanghao11.cn/gthmrnbkzi.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtzgckwxfa.html

C#:   7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtojizjwia.html

[A06] 字符串转数字
来源：http://hz.sxryk.cn/gtgzbytuou.html

Py:   int("42"); float("3.14")
来源：http://hz.zycfv.cn/gteloygoqx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.52xcode.cn/gtlxybztux.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.316326.xyz/gtfqkwgzkf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhixingplan.top/gtsgpugdzh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nwbrower.top/gtditzbmyn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sysykeji.top/gtdyizzyck.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yueranfly.top/gthlrwhhvs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.andypj.xyz/gtwvdbpoos.html

[A07] 数字转字符串
来源：http://hz.yuxming.cn/gtncxagmtp.html

Py:   str(42)
来源：http://hz.cqqwz.cn/gtpsywhsat.html

PHP:  (string) 42; strval(42)
来源：http://hz.cdnleiting.top/gtkrhbzstn.html

JS:   String(42); (42).toString()
来源：http://hz.jinghuilouyu.cn/gtatmgqbmc.html

TS:   String(42)
来源：http://hz.zhongyouzk.top/gtzqzcwfvj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jinqigfzy.top/gtbotkzgjk.html

Go:   strconv.Itoa(42)
来源：http://hz.yongpay.top/gtbnaxgkps.html

Ruby: 42.to_s
来源：http://hz.hysaishi.cn/gtkujmhzsj.html

C#:   42.ToString()
来源：http://hz.nwbrower.top/gtnpzqimnm.html

[A08] 取整与四舍五入
来源：http://hz.xingfuxueyuan.xyz/gtknnamkoz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aibaodan.cn/gtiazkplkr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.redwolf501.top/gtmfgehtkz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.tian-w.cn/gthgkagcys.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.wangdashe.top/gtdkuihirq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.316326.xyz/gthqeihekg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtjsyslheh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cucudq.cn/gtexeuqeaa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.52xcode.cn/gtcvqteagb.html

[A09] 绝对值与最大最小值
来源：http://hz.xuetiantiany.cn/gttayxnshy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aizwys.cn/gtxmtympkt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gtdizdoltq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zycfv.cn/gtyvsxcsfo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.c1oappe.top/gtlqgqyowk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.52xcode.cn/gtpbmtayrg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.shanyushiyangtech.top/gtnyrqjupz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yuanzhike.top/gteatllicu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hnxiangtu.top/gtybdqnimh.html

[A10] 生成随机数
来源：http://hz.nanxuanxn.top/gtyomdvmjq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hfpthk.cn/gtlkvjsnak.html

PHP:  random_int(1, 100);
来源：http://hz.xylfe.cn/gtntkqnzfh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yanxiufei.cn/gtvegtpbps.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangdashe.top/gtyhrtagif.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hfpthk.cn/gtlmymqxvx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yueranfly.top/gtnjhfspbe.html

Ruby: rand(1..100)
来源：http://hz.sweek.top/gtxhbazaog.html

C#:   new Random().Next(1, 101)
来源：http://hz.jinqigufen.top/gtpqrlejxd.html

[A11] 条件表达式（三元）
来源：http://hz.jiagoushi.top/gtjezjxkdx.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hywenlv.cn/gtbvlamfeu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtcezmesea.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtjtyxehjn.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.xuetiantiany.cn/gtjruiaooo.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtlptqgcxh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gaohongyu789.top/gtajbqeghm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtvhlzztnd.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.cdnleiting.top/gthwuuvqqz.html

[A12] 字符串插值 / 格式化
来源：http://hz.xuanzx.com/gtcgcwyhru.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.vqdsnc.cn/gtmhuduiji.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.quarkkingdee.top/gtnlwfsofc.html

JS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gtfsbzfize.html

TS:   `Hello, ${name}!`
来源：http://hz.yj202588.top/gttoperswk.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yj20258.top/gtnhmpyojy.html


<!-- 参考信息 -->