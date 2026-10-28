代发 wailian999

[U79] PHP：静态分析
来源：http://hz.zhaomingkeji.xyz/gtvyjrmasv.html

composer require --dev phpstan/phpstan
来源：http://hz.nwbrower.top/gtgszpxtem.html

[U80] PHP：代码规范修复
来源：http://hz.jinqigfzy.top/gtktovvsqa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtfjndtjub.html

[U81] JS：初始化项目
来源：http://hz.shuidangran.top/gtbdnxiyhb.html

npm init -y;  npm i express
来源：http://hz.quarkkingdee.top/gtyevkczft.html

[U82] JS：package.json 脚本
来源：http://hz.jinghuilouyu.cn/gtpxyvjrqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.c1oappe.top/gtqqnycfyr.html

[U83] JS：ES Module 导入导出
来源：http://hz.tanke756.top/gtcgqaqgww.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jlsjyb.cn/gtncambkag.html

[U84] JS：CommonJS 写法
来源：http://hz.yj20258888.top/gtqdlfpuqw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtjnddrxbk.html

[U85] JS：可选链
来源：http://hz.zhongyouzk.top/gtwzkfvyjc.html

a?.b?.c
来源：http://hz.kuanghao11.cn/gtaeoapvwj.html

[U86] JS：空值合并
来源：http://hz.kuanghao11.cn/gtbzbuyvyw.html

a ?? b
来源：http://hz.cqqwz.cn/gtsmpoopgx.html

[U87] JS：解构默认值
来源：http://hz.chenjidiqi.icu/gtsabvanqe.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cashguo.top/gtkryezihu.html

[U88] JS：对象展开合并
来源：http://hz.tianlin.xyz/gtzydhixxz.html

{ ...a, ...b }
来源：http://hz.jlsjyb.cn/gtfndpbprt.html

[U89] JS：数组去重
来源：http://hz.sufxvd.cn/gtrxwmsanw.html

[...new Set(arr)]
来源：http://hz.zhijiandao.cn/gthakdobyh.html

[U90] JS：数字数组排序
来源：http://hz.zhiwuduotai.top/gtylleuhog.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gthtkfgzms.html

[U91] JS：对象键值遍历
来源：http://hz.dianchejie.cn/gtjnrgfsia.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shzxlz.cn/gtuakypheg.html

[U92] JS：深拷贝
来源：http://hz.zhoulong.xyz/gtnbeqwnuz.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtdcqejsyg.html

[U93] JS：模板字符串
来源：http://hz.tian-w.cn/gtsevuobqk.html

`共 ${n} 条`
来源：http://hz.aibaodan.cn/gtlgsszbop.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtlkwlqshl.html

const double = x => x * 2;
来源：http://hz.hfpthk.cn/gtfiynmxzr.html

[U95] JS：Promise 包装
来源：http://hz.chenjidiqi.icu/gthiodhipr.html

new Promise((resolve, reject) => {})
来源：http://hz.xinyue.icu/gtntdwdxal.html

[U96] JS：async/await 与异常
来源：http://hz.pengpengdd.cyou/gtihrnmbzi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtujrhsifs.html

[U97] JS：并发请求
来源：http://hz.zhiwuduotai.top/gtxexqyeso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtyuxzizvz.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydjk.org.cn/gtxiwsomdy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tianlin.xyz/gtbnbntlgy.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gtpmciynhn.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtrqxopuom.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gtlzqdnxnx.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gtuejllcdk.html

[U101] JS：classList 操作
来源：http://hz.tanke756.top/gtrfgquael.html

el.classList.toggle("active")
来源：http://hz.cucudq.cn/gtocxssxff.html

[U102] JS：本地存储
来源：http://hz.tianlin.xyz/gtbufdffvo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ppjwa.cn/gtsomwkkcp.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gttiaitjfy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aibaodan.cn/gtztfdzqhh.html

[U104] JS：防抖
来源：http://hz.havefunace.top/gtyyejbrws.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtgckwxprt.html

[U105] JS：节流
来源：http://hz.zhixingplan.top/gtablbagvo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhaomingkeji.xyz/gttcbufhts.html

[U106] JS：日期格式化
来源：http://hz.52xcode.cn/gtnymkpdbj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.birdmap.top/gtyvynxaqr.html

[U107] JS：数字千分位
来源：http://hz.zhiwuduotai.top/gtjnohegpq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtvoluezhx.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gtcmdismqa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuetiantiany.cn/gttyckxqig.html

[U109] JS：数组分组
来源：http://hz.fzhhl.top/gtndvkebjl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtkbnfprid.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtoozissrf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.wangshuangyany.cn/gtxdnwwqws.html

[U111] JS：对象转 Map
来源：http://hz.shzxlz.cn/gtnzfpglkh.html

new Map(Object.entries(obj))
来源：http://hz.daxiang520.top/gtatwjmtfp.html

[U112] JS：字符串补位
来源：http://hz.yvedp.cn/gthvzbtdvo.html

"7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtybzijidc.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangtech.top/gtwkielriy.html

s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtiqlguvof.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gtuqspgojc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtxxwbeahk.html

[U115] JS：生成 UUID
来源：http://hz.shanyushiyangtech.top/gtneugscix.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtvmpwhing.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxuanxn.top/gtdsaamjig.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtwmufxmah.html

[U117] JS：单元测试
来源：http://hz.yuxming.cn/gtvybskcjl.html

npm i -D vitest;  npx vitest
来源：http://hz.ywan-chungtsiang.top/gtttrfksno.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtobyvwweb.html

npm i -D vite;  npx vite
来源：http://hz.zycfv.cn/gtefdcswuo.html

[U119] JS：生产构建
来源：http://hz.zhoulong.xyz/gthkhdnwny.html

npx vite build
来源：http://hz.kuanghao11.cn/gtuevjwhfk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gogol.net.cn/gtklgvllec.html

import.meta.env.VITE_API_URL
来源：http://hz.jinyuanbaomall.cn/gtvcszmtze.html

================================================================================
来源：http://hz.quarkkingdee.top/gtteiodeut.html

统计汇总
来源：http://hz.yongpay.top/gtksukqctz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvzqzrsmg.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtfjbgbubj.html

Python ......... 252
来源：http://hz.iojbl.cn/gtyamujnyw.html

PHP ............ 252
来源：http://hz.ehwqpu.com/gtljqeycar.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtrexekplw.html

TypeScript ..... 212
来源：http://hz.fengsongda.top/gtqsohwpnx.html

Java ........... 212
来源：http://hz.pycfn.com/gtftjboige.html

Go ............. 212
来源：http://hz.316326.xyz/gtdeepoojs.html

Ruby ........... 212
来源：http://hz.yvedp.cn/gtlyqhjing.html

C# ............. 212
来源：http://hz.iojbl.cn/gtlkpfetug.html

C .............. 30
来源：http://hz.yvedp.cn/gtjlwxexvf.html

C++ ............ 30
来源：http://hz.yonumen.top/gtstsqgldj.html

SQL ............ 90
来源：http://hz.pycfn.com/gtkpcrdhek.html

Bash ........... 80
来源：http://hz.vqdsnc.cn/gtuohafmmi.html

Kotlin ......... 15
来源：http://hz.cucudq.cn/gtektvtzjw.html

Swift .......... 15
来源：http://hz.wangshuangyany.cn/gtjsomfdsg.html

Lua ............ 10
来源：http://hz.havefunace.top/gtyehtjeme.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtacdtnohs.html

Scala .......... 10
来源：http://hz.svipenyu.cn/gthegrcbvd.html

------------------------------------
来源：http://hz.chenlongwang.top/gtcgqholnl.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtyhywpbvu.html

按章节统计：
来源：http://hz.jqgfzy.top/gtswpqmjti.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtxttwkzxr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtbsealxzq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtvhgekhty.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtjkzdogwg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gtizkwqtyw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gtfnlmvqks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtitecxofp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuxming.cn/gtrdsfntnb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtgvtyuhdt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtxkafvvpe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtzppydjjf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtqiorkahp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtymzqjvwo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.tanke756.top/gtuzloxtne.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenlongwang.top/gtqtdoimsp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtrswjngun.html

Q SQL 专题                              90
来源：http://hz.xziqi.cn/gtskrzpnsw.html

R Bash 专题                             80
来源：http://hz.quarkkingdee.top/gttklrnmsa.html

S C / C++ 专题                          60
来源：http://hz.0kj1m.cn/gtgkqcmrss.html

T 其他语言补充                          60
来源：http://hz.andypj.xyz/gtqqtklkty.html

U 高频实用片段                         120
来源：http://hz.gaohongyu789.top/gtorpxszya.html

------------------------------------
来源：http://hz.zycfv.cn/gtnlrajdet.html

合计                                  2106 条
来源：http://hz.hammf.cn/gtlbyyrfjk.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gttmhqbpra.html

使用提醒
来源：http://hz.gotoacloud.top/gtzgnrlssr.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtfehutexd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.aizwys.cn/gtgnpoansu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xinyue.icu/gtrxsbfril.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ywan-chungtsiang.top/gtnyydpwur.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenlongwang.top/gtacsslatg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xylfe.cn/gtatebitur.html

—— 文件结束 ——
来源：http://hz.xingfuxueyuan.xyz/gtjqhgsslz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwimupozl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zycfv.cn/gtjvytgktd.html

Common Programming Examples Cheat Book
来源：http://hz.yuanzhike.top/gtnshvaxom.html

================================================================================
来源：http://hz.ehwqpu.com/gtotjckglk.html

【收录内容】
来源：http://hz.yuanzhike.top/gtsotjwcim.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hongshengwenyu.top/gtqpfcsbag.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gogol.net.cn/gtxkumyhra.html

SQL · Bash · C · C++
来源：http://hz.xuetiantiany.cn/gtymixglhc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yanxiufei.cn/gtkqccjhpm.html

【使用说明】
来源：http://hz.zdqjudy.top/gtgwfczarh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.pycfn.com/gtujfrlqzq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gzhubu.top/gtdyfbcxbj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gtafsnntou.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtonnqteyj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ehwqpu.com/gtykjfngjr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258888.top/gthqholqnz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gtbiyfglyj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.havefunace.top/gtcxlwyvbf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xuanzx.com/gtahfcqyqo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ehwqpu.com/gtsmomsmsx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hammf.cn/gtriingcly.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhengqikj.top/gtupnvszvf.html

【文件统计】
来源：http://hz.haohaochexian.top/gtrngawqex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yuanzhike.top/gtsbvwheez.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gtvwginjce.html

目  录
来源：http://hz.wangdashe.top/gtmpklbyhg.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gthjxydpjx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.sweek.top/gtfzaacdnu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtmusxwnxt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtmmrcfwqk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hfpthk.cn/gtygesytky.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xingfuxueyuan.xyz/gtukpxoqeb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtgccxlpkm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtcdinyxzc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtqouwgfoy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtgzothsxc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhiwuduotai.top/gtkrtndydy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtfecsswxo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtnyexdwsj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtfsgdrjnj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtlocgruaf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ppjwa.cn/gtpkvyzmux.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtvomhwmtl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhoulong.xyz/gtkmmexozr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinyuanbaomall.cn/gtowjcxazb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sweek.top/gtusrfjped.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtadzdwioi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtnagwefei.html

================================================================================
来源：http://hz.yj20258.top/gtzjxqexdv.html

A. 基础语法与类型
来源：http://hz.ywan-chungtsiang.top/gtgwttoypl.html

================================================================================
来源：http://hz.9152youxi.cn/gtjntjlava.html

[A01] Hello World
来源：http://hz.hysaishi.cn/gtzrjpdtab.html

Py:   print("Hello, World!")
来源：http://hz.c1oappe.top/gteqoexglt.html

PHP:  echo "Hello, World!";
来源：http://hz.9152youxi.cn/gtvzivvfyy.html

JS:   console.log("Hello, World!");
来源：http://hz.dashuyun.cn/gtlyfljbpn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sufxvd.cn/gtckbwiqak.html

Java: System.out.println("Hello, World!");
来源：http://hz.mhx1999.top/gtxswxermk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yueranfly.top/gttlrhmwdv.html

Ruby: puts "Hello, World!"
来源：http://hz.zhongyouzk.top/gtxxnigekc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenlongwang.top/gtofbpildl.html

[A02] 变量声明与赋值
来源：http://hz.hywenlv.cn/gtegldnjuk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.0kj1m.cn/gtnwzugajs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gaohongyu789.top/gtjxqcdska.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.fzhhl.top/gtzahocoen.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.smart0.xyz/gtpxjpjeqv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xylfe.cn/gtvljqfprs.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gtzufifpni.html

Ruby: name = "Alex"; age = 20
来源：http://hz.316326.xyz/gtejnclnwg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtigjeyxus.html

[A03] 常量定义
来源：http://hz.hysaishi.cn/gtfeqnkudj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jianghu66.top/gtxmwpynpg.html

PHP:  const PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtpsqcqulv.html

JS:   const PI = 3.14159;
来源：http://hz.yongpay.top/gturbawrbk.html

TS:   const PI: number = 3.14159;
来源：http://hz.cucudq.cn/gtxeddwvda.html

Java: static final double PI = 3.14159;
来源：http://hz.smart0.xyz/gtyveqkkew.html

Go:   const PI = 3.14159
来源：http://hz.xinyue.icu/gtzfdscedy.html

Ruby: PI = 3.14159
来源：http://hz.yanxiufei.cn/gtaeltobpr.html

C#:   const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtibhcixxb.html

[A04] 判断变量类型
来源：http://hz.cheryme.top/gtqywsaomp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jlsjyb.cn/gtmbprwhvz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.mhx1999.top/gtikcmenvz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.smart0.xyz/gtdmrqtlph.html

TS:   typeof x; x instanceof Date
来源：http://hz.9152youxi.cn/gtmmpjsjec.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hfpthk.cn/gtzrekslxp.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.316326.xyz/gtxfpnkmnw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.chenjidiqi.icu/gtakunmmsh.html

C#:   x.GetType().Name; x is int
来源：http://hz.svipenyu.cn/gtyqejylsf.html

[A05] 整数除法与取模
来源：http://hz.jinyuanbaomall.cn/gtategqzow.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ybcxt.top/gtzmccguic.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hfpthk.cn/gtkcrjakky.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtfaiobxfq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yuanzhike.top/gttslerzqj.html

Java: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gthzdckpwt.html

Go:   7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gtfoujbiao.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtdjnyhtcb.html

C#:   7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtnzhjrkkn.html

[A06] 字符串转数字
来源：http://hz.jqgfzy.top/gtbvefzhpx.html

Py:   int("42"); float("3.14")
来源：http://hz.zhoulong.xyz/gtbchfjbhh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydjk.org.cn/gtthjphkax.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yueranfly.top/gtpqafyisg.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtpbfvjiwm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinghuilouyu.cn/gtssgylbka.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gotoacloud.top/gttstittea.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hongshengwenyu.top/gtxcgabwec.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.sufxvd.cn/gtrnmimgkw.html

[A07] 数字转字符串
来源：http://hz.ydzc1.top/gtzpsqwjje.html

Py:   str(42)
来源：http://hz.kuanghao11.cn/gtkfbyqhgc.html

PHP:  (string) 42; strval(42)
来源：http://hz.redwolf501.top/gtorplwtnz.html

JS:   String(42); (42).toString()
来源：http://hz.zhiwuduotai.top/gtniqrxpgd.html

TS:   String(42)
来源：http://hz.hfpthk.cn/gtfdtnuvks.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shangyingyoupin.top/gtqvbzbdgq.html

Go:   strconv.Itoa(42)
来源：http://hz.wangshuangyany.cn/gtlsyplngy.html

Ruby: 42.to_s
来源：http://hz.shuidangran.top/gtjmpgorqv.html

C#:   42.ToString()
来源：http://hz.iojbl.cn/gtdrmjcwgj.html

[A08] 取整与四舍五入
来源：http://hz.gaohongyu789.top/gtgmpqxkmg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aibaodan.cn/gttumenypt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.c1oappe.top/gtvytwffbi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.daxiang520.top/gtczehmeid.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yuxming.cn/gtbqbtejgm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.c1oappe.top/gtslyxzdou.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.redwolf501.top/gtqfmvnruf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.aibaodan.cn/gtwyolvkus.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nanxuanxn.top/gtjrfpyvma.html

[A09] 绝对值与最大最小值
来源：http://hz.hfpthk.cn/gtwessiqwp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gtfereakfy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nwbrower.top/gtrnwjugkn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhengqikj.top/gtpxgbikei.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtalczopgp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xziqi.cn/gtyijpbfmt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cheryme.top/gtjdcqinmr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.redwolf501.top/gtbssqwdiz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hywenlv.cn/gtmqfycqez.html

[A10] 生成随机数
来源：http://hz.sxryk.cn/gtvrgglnwt.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhongyouzk.top/gtbwvedpqr.html

PHP:  random_int(1, 100);
来源：http://hz.aizwys.cn/gtloqeijba.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shanyushiyangkeji.top/gtggbhpvum.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cqqwz.cn/gtwjnengyi.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gzhubu.top/gtpshhdaxc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.chenzaomai.com/gtptkjkqqt.html

Ruby: rand(1..100)
来源：http://hz.yangfankeji.com/gtwxxtqfhv.html

C#:   new Random().Next(1, 101)
来源：http://hz.xuetiantiany.cn/gtrbglwsra.html

[A11] 条件表达式（三元）
来源：http://hz.yj20258.top/gtypcybssa.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.chenlongwang.top/gtmhstrsiq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xuanzx.com/gtlsvtavdr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.meibo888.top/gtacdnlhne.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtrhzxjpps.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtoqjxsybz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.nanxuanxn.top/gtvkdpcqwh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtkrampkut.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtyorrqgdy.html

[A12] 字符串插值 / 格式化
来源：http://hz.xziqi.cn/gtoklmhwqs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jinqigfzy.top/gttayjgzwb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.quarkkingdee.top/gthbarbdkn.html

JS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gtpvxsbhzp.html

TS:   `Hello, ${name}!`
来源：http://hz.yj20258888.top/gtdkhniopa.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jiagoushi.top/gtdbqlwgus.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhixingplan.top/gtoelntvem.html

Ruby: "Hello, #{name}!"
来源：http://hz.gzhubu.top/gtlofloqge.html

C#:   $"Hello, {name}!"
来源：http://hz.0kj1m.cn/gtufeusvhf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cashguo.top/gtoboomoyt.html


<!-- 参考信息 -->