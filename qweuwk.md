代发 wailian999

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtnygeqtni.html

composer require --dev phpstan/phpstan
来源：http://hz.shanyushiyangtech.top/gtlpnqjifq.html

[U80] PHP：代码规范修复
来源：http://hz.ydzc1.top/gttuprzkbu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hysaishi.cn/gtorjqrruc.html

[U81] JS：初始化项目
来源：http://hz.zhiwuduotai.top/gtwtkbqgow.html

npm init -y;  npm i express
来源：http://hz.cashguo.top/gtvqygdcag.html

[U82] JS：package.json 脚本
来源：http://hz.nwbrower.top/gtusqwxnyo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtyauuuefy.html

[U83] JS：ES Module 导入导出
来源：http://hz.dashuyun.cn/gtznqdhczk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gthrghdttw.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtixmsezsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sufxvd.cn/gtisbjxlli.html

[U85] JS：可选链
来源：http://hz.xinyue.icu/gtgfgurxgw.html

a?.b?.c
来源：http://hz.wangshuangyany.cn/gtebgitfhr.html

[U86] JS：空值合并
来源：http://hz.jinyuanbaomall.cn/gtmkbgnmjn.html

a ?? b
来源：http://hz.xuanzx.com/gterbqgnth.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gtbvkiedsq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.vqdsnc.cn/gteggrnnbx.html

[U88] JS：对象展开合并
来源：http://hz.aibaodan.cn/gtfiklfhuq.html

{ ...a, ...b }
来源：http://hz.ppjwa.cn/gtckugpcou.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtmwdtfrta.html

[...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtlsygvuuk.html

[U90] JS：数字数组排序
来源：http://hz.jinqigufen.top/gtnkuqequr.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtthvzosrb.html

[U91] JS：对象键值遍历
来源：http://hz.quarkkingdee.top/gthcxzdrwk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj202588.top/gtqrbibapn.html

[U92] JS：深拷贝
来源：http://hz.birdmap.top/gtnkqqyjkf.html

structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtyailcqiu.html

[U93] JS：模板字符串
来源：http://hz.xylfe.cn/gtacrhqcag.html

`共 ${n} 条`
来源：http://hz.haohaochexian.top/gtmasclwlk.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtyffzybpu.html

const double = x => x * 2;
来源：http://hz.andypj.xyz/gtezaktjiq.html

[U95] JS：Promise 包装
来源：http://hz.yuanzhike.top/gtorjcntwg.html

new Promise((resolve, reject) => {})
来源：http://hz.xinyue.icu/gtyoerhpjt.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtdokwfmrn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtpueoahof.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtdmjucnus.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtwtxbkxoe.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhiwuduotai.top/gteginrkyy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.0kj1m.cn/gtnogyxrrd.html

[U99] JS：事件监听
来源：http://hz.xziqi.cn/gtivmtdkvr.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gtzjrctnfu.html

[U100] JS：DOM 查询
来源：http://hz.fzhhl.top/gtbpwejyfr.html

document.querySelector(".item")
来源：http://hz.yonumen.top/gtcphzuddn.html

[U101] JS：classList 操作
来源：http://hz.cqqwz.cn/gtenaqbbdx.html

el.classList.toggle("active")
来源：http://hz.zhiwuduotai.top/gtjyottwxm.html

[U102] JS：本地存储
来源：http://hz.jqgufenzy.top/gtnwnedzkk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dashuyun.cn/gtyluuzqbf.html

[U103] JS：定时器
来源：http://hz.xingfuxueyuan.xyz/gtjqfnulhi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtqxffeazb.html

[U104] JS：防抖
来源：http://hz.aibaodan.cn/gtpcndfaub.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gteektdahc.html

[U105] JS：节流
来源：http://hz.zhongyouzk.top/gtodswhvbp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daria6918.cn/gtmpqxtetk.html

[U106] JS：日期格式化
来源：http://hz.jinghuilouyu.cn/gtsrvidumd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hywenlv.cn/gtucvnhjat.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtzokgvrtr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yongpay.top/gtqqicrkkb.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtrgynehxz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aibaodan.cn/gtbvilyire.html

[U109] JS：数组分组
来源：http://hz.gzhubu.top/gtglneklft.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtuzrjyqip.html

[U110] JS：数组分块
来源：http://hz.cqqwz.cn/gtrgocugkj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cheryme.top/gtcoewcbxr.html

[U111] JS：对象转 Map
来源：http://hz.9152youxi.cn/gtmzlotzfa.html

new Map(Object.entries(obj))
来源：http://hz.daria6918.cn/gtvajvfnwi.html

[U112] JS：字符串补位
来源：http://hz.zhongyouzk.top/gthbsbdfzz.html

"7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtxnxkjsqi.html

[U113] JS：正则替换全部
来源：http://hz.shangyingyoupin.top/gtadjutmhc.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtekqngxlj.html

[U114] JS：JSON 深比较
来源：http://hz.gogol.net.cn/gtwjvequgc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtvjmpwwrw.html

[U115] JS：生成 UUID
来源：http://hz.bjfxy.top/gtvfhwxqsr.html

crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtfwdtncxv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhiwuduotai.top/gtirtfgmar.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hywenlv.cn/gtsomqsrhc.html

[U117] JS：单元测试
来源：http://hz.zdqjudy.top/gtcajpbirp.html

npm i -D vitest;  npx vitest
来源：http://hz.cashguo.top/gtflzznrgm.html

[U118] JS：开发服务器
来源：http://hz.tian-w.cn/gtblctknpr.html

npm i -D vite;  npx vite
来源：http://hz.shzxlz.cn/gtrqciekyd.html

[U119] JS：生产构建
来源：http://hz.tianlin.xyz/gtnhymcqea.html

npx vite build
来源：http://hz.jinqigufen.top/gtvrwdexge.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sysykeji.top/gtzvdkesnk.html

import.meta.env.VITE_API_URL
来源：http://hz.gaohongyu789.top/gtdhzncbbr.html

================================================================================
来源：http://hz.pycfn.com/gtsypqtjjq.html

统计汇总
来源：http://hz.ehwqpu.com/gtmtgmpigq.html

================================================================================
来源：http://hz.guowangkeji.top/gtehuqoqub.html

按语言统计（条）：
来源：http://hz.dashuyun.cn/gtpfgzwsdi.html

Python ......... 252
来源：http://hz.ydzc1.top/gtawcgltol.html

PHP ............ 252
来源：http://hz.cqqwz.cn/gtvjbbuvwd.html

JavaScript ..... 252
来源：http://hz.dianchejie.cn/gthylfkboz.html

TypeScript ..... 212
来源：http://hz.jinqigfzy.top/gtccdeisza.html

Java ........... 212
来源：http://hz.ppjwa.cn/gthyujptqf.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtbeegjgeh.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtdoifhzta.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gttublsbln.html

C .............. 30
来源：http://hz.hysaishi.cn/gttwnofvkx.html

C++ ............ 30
来源：http://hz.tanke756.top/gtwsmcytvu.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtiozkzgfo.html

Bash ........... 80
来源：http://hz.yangfankeji.com/gtkeezgofo.html

Kotlin ......... 15
来源：http://hz.jqgufenzy.top/gtloaroxwt.html

Swift .......... 15
来源：http://hz.shzxlz.cn/gtixeaxenw.html

Lua ............ 10
来源：http://hz.zycfv.cn/gthhzildqu.html

Perl ........... 10
来源：http://hz.jianghu66.top/gtsxngikbk.html

Scala .......... 10
来源：http://hz.guowangkeji.top/gtjoduyrvw.html

------------------------------------
来源：http://hz.xylfe.cn/gtysfvwhqi.html

合计 ........... 2106 条
来源：http://hz.tian-w.cn/gttzznbywt.html

按章节统计：
来源：http://hz.zhoulong.xyz/gtxaokponh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cheryme.top/gtdmcsqgtz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.gzhubu.top/gtoqljjqhd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gthnzntdcb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yuxming.cn/gtaboarvom.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhijiandao.cn/gthmjczahk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtdevyvqyo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtjixmgcgz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhongyouzk.top/gtquzhemmo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtbipsxkok.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtsgfugwyf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtenajknfm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtwvkzljiy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtiodfdwya.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtaixzgaqc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.52xcode.cn/gtthwyyvnp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gterirnogf.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gtsdvrnlrj.html

R Bash 专题                             80
来源：http://hz.jlsjyb.cn/gtqlezoxwn.html

S C / C++ 专题                          60
来源：http://hz.chenjidiqi.icu/gtnrwwvwjb.html

T 其他语言补充                          60
来源：http://hz.nwbrower.top/gtaaojtqqg.html

U 高频实用片段                         120
来源：http://hz.andypj.xyz/gtbvawetoq.html

------------------------------------
来源：http://hz.meibo888.top/gtugcacdwt.html

合计                                  2106 条
来源：http://hz.chenzaomai.com/gtsrhktrzg.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtqiljxyry.html

使用提醒
来源：http://hz.yangfankeji.com/gtnslffpua.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtmkwskfto.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.tianlin.xyz/gtgmcgxrcn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ivvv.top/gtekxeaglp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cashguo.top/gtamzrxxqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ivvv.top/gtvscrzfxk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ivvv.top/gthxvbkepj.html

—— 文件结束 ——
来源：http://hz.hysaishi.cn/gtarvvjdxi.html

================================================================================
来源：http://hz.cucudq.cn/gtpeidbmfj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhongyouzk.top/gtkccqvihv.html

Common Programming Examples Cheat Book
来源：http://hz.zdqjudy.top/gtcbefbeyq.html

================================================================================
来源：http://hz.sxryk.cn/gtrlpbfmdw.html

【收录内容】
来源：http://hz.fzhhl.top/gthkdjthwg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.iojbl.cn/gtlrqhizqr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydzc1.top/gtvklvmiuv.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtxzlukxfi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shangyingyoupin.top/gtpndvidku.html

【使用说明】
来源：http://hz.shzxlz.cn/gtujbznikr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.bjfxy.top/gtcqvbaqrt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.svipenyu.cn/gtbmxmqbgf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.daxiang520.top/gtxpkvmifn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jiagoushi.top/gtqxkdbjoz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinyuanbaomall.cn/gtejkmcwdg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jqgfzy.top/gtlxvvhkma.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.daria6918.cn/gtsodmppxy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yonumen.top/gtsrjgsdif.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.dianchejie.cn/gtphakrqzu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fzhhl.top/gtpkuqtcxa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgufenzy.top/gtwwtwglcz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jianghu66.top/gtwlrxdnvb.html

【文件统计】
来源：http://hz.ydzc1.top/gtdyvbkeoi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yangfankeji.com/gtzjemppoz.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtsyqeupgt.html

目  录
来源：http://hz.xylfe.cn/gtrmujnobh.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtrfeqhdui.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtnzkvukzz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jianghu66.top/gtxbxzozzp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gttfrmdjyo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shuidangran.top/gtwatztyax.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cdnleiting.top/gtwewxynbf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtolxfanyp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtjweqyjis.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gtmfhhfxmk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtwgidllsf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtdosifzhs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtezqpdpuq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtjnczmjsj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gttujkcakv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gtbkdvhcgh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinyuanbaomall.cn/gtgsrlwxox.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtgvkfbolv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhoulong.xyz/gtocthlguk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nwbrower.top/gtmcxolrjt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jinqigufen.top/gtfutwpbwr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xinyue.icu/gtqvyyxviy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtyregxqup.html

================================================================================
来源：http://hz.hfpthk.cn/gtslamadwz.html

A. 基础语法与类型
来源：http://hz.jinghuilouyu.cn/gteasfkemk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnplfogvt.html

[A01] Hello World
来源：http://hz.fzhhl.top/gtncguhevq.html

Py:   print("Hello, World!")
来源：http://hz.yanxiufei.cn/gtyistqoge.html

PHP:  echo "Hello, World!";
来源：http://hz.mhx1999.top/gtbbamowiu.html

JS:   console.log("Hello, World!");
来源：http://hz.zhoulong.xyz/gtsrgbozyq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.redwolf501.top/gtgeeolaew.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtdulfnzqf.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.snrcjt.cn/gtanphjufr.html

Ruby: puts "Hello, World!"
来源：http://hz.ybcxt.top/gtdqojszjh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yvedp.cn/gtubmwlgmg.html

[A02] 变量声明与赋值
来源：http://hz.hysaishi.cn/gtvubrxwfy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yj20258.top/gtcjsohuca.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sxryk.cn/gtmtlwaqxi.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenjidiqi.icu/gtrpwxxibf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yonumen.top/gttqopgzun.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.snrcjt.cn/gtbcbuhnyt.html

Go:   name := "Alex"; age := 20
来源：http://hz.ydjk.org.cn/gtyxdsaewu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnqzz.top/gtxrmjiazf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xuanzx.com/gtymggvcmo.html

[A03] 常量定义
来源：http://hz.xuetiantiany.cn/gtmdjqpfkx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.daria6918.cn/gtexqmhqwp.html

PHP:  const PI = 3.14159;
来源：http://hz.9152youxi.cn/gtzkqvcayv.html

JS:   const PI = 3.14159;
来源：http://hz.xinyue.icu/gtivrpvpaq.html

TS:   const PI: number = 3.14159;
来源：http://hz.shzxlz.cn/gtjtiafemh.html

Java: static final double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtdseebxyk.html

Go:   const PI = 3.14159
来源：http://hz.hammf.cn/gtnickrkpy.html

Ruby: PI = 3.14159
来源：http://hz.xinyue.icu/gtelpuansu.html

C#:   const double PI = 3.14159;
来源：http://hz.yongpay.top/gtxzrdwyck.html

[A04] 判断变量类型
来源：http://hz.zycfv.cn/gterhykgai.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yonumen.top/gtgyzwskhp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sysykeji.top/gttbidlhkd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ivvv.top/gtfwcjrvxn.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinghuilouyu.cn/gtbenjqrvv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.redwolf501.top/gtrxqrjuep.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.smart0.xyz/gtmxlxapgf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zycfv.cn/gtwauoyvrz.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinghuilouyu.cn/gtvbsudjyn.html

[A05] 整数除法与取模
来源：http://hz.sysykeji.top/gtxtcqzopk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhaomingkeji.xyz/gtddzngknv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtwcvalhtw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xziqi.cn/gtxylvqnfk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtqoadlwie.html

Java: 7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtzmrgymem.html

Go:   7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gtohjkrgwb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtqdmjnctx.html

C#:   7 / 2; 7 % 2
来源：http://hz.ehwqpu.com/gtlymnrkck.html

[A06] 字符串转数字
来源：http://hz.chenjidiqi.icu/gteauselwv.html

Py:   int("42"); float("3.14")
来源：http://hz.tanke756.top/gtvkxiknqz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhixingplan.top/gtmkwxrthu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ybcxt.top/gtfrkoadah.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guowangkeji.top/gtnrapnfqz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhongyouzk.top/gttwvodtpw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.fzhhl.top/gtfzsdzfvi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yvedp.cn/gtxqsjwlmf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.daria6918.cn/gthiwnhbkx.html

[A07] 数字转字符串
来源：http://hz.nwbrower.top/gtiowuyamg.html

Py:   str(42)
来源：http://hz.ydjk.org.cn/gtcyyihnod.html

PHP:  (string) 42; strval(42)
来源：http://hz.hongshengwenyu.top/gtmkoqyizp.html

JS:   String(42); (42).toString()
来源：http://hz.havefunace.top/gtbfgdvmvb.html

TS:   String(42)
来源：http://hz.pycfn.com/gtivflxqsw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sxryk.cn/gtythqxztp.html

Go:   strconv.Itoa(42)
来源：http://hz.aibaodan.cn/gtovexuzea.html

Ruby: 42.to_s
来源：http://hz.shanyushiyangkeji.top/gtnglxusgs.html

C#:   42.ToString()
来源：http://hz.shanyushiyangkeji.top/gtugnonfni.html

[A08] 取整与四舍五入
来源：http://hz.cheryme.top/gtvjxkkqyc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.tian-w.cn/gtopknekvc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gogol.net.cn/gtoiskyglo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.chenlongwang.top/gtsfdsopsv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhijiandao.cn/gttzjcgdtn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nwbrower.top/gtxqujioep.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.xuetiantiany.cn/gtdgpzpdmz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.tian-w.cn/gtyqgyxogl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtqfrhudif.html

[A09] 绝对值与最大最小值
来源：http://hz.jiagoushi.top/gtxdfkbqbf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gtntqxkwpd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ybcxt.top/gtfigkysgo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.gaohongyu789.top/gtskmvxtts.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.guowangkeji.top/gtytgjbrcc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.yj202588.top/gtotslqvcd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jlsjyb.cn/gtsqhbbxch.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.daxiang520.top/gtaimmfhcd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.haohaochexian.top/gtqcnglqeb.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtqehglmgb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.sufxvd.cn/gtcfxzrlqx.html

PHP:  random_int(1, 100);
来源：http://hz.nanxinkj.top/gtvglmzxdt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuxming.cn/gtohjeaany.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.tianlin.xyz/gtaoyzbxbk.html

Java: new Random().nextInt(100) + 1
来源：http://hz.meibo888.top/gtwfnexmoj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.nanxuanxn.top/gtherkqwrb.html

Ruby: rand(1..100)
来源：http://hz.mhx1999.top/gtihzcnzaw.html

C#:   new Random().Next(1, 101)
来源：http://hz.guowangkeji.top/gtuoffjxfg.html

[A11] 条件表达式（三元）
来源：http://hz.snrcjt.cn/gtmcdhczfx.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hammf.cn/gtwhwyeqma.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.snrcjt.cn/gtkpjmkyll.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.wangshuangyany.cn/gtfsdicjtl.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtaddohwui.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtzejkzqvy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sweek.top/gtybslqprl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtsjvsqzrm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtjhtpsath.html

[A12] 字符串插值 / 格式化
来源：http://hz.jyoumei.cn/gtoxcghadp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jyoumei.cn/gtxxzokrtr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jinqigufen.top/gtyvotdpzh.html

JS:   `Hello, ${name}!`
来源：http://hz.ywan-chungtsiang.top/gtzsekgwbe.html

TS:   `Hello, ${name}!`
来源：http://hz.pycfn.com/gtchcqvork.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jinyuanbaomall.cn/gtjpwvqnqj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhengqikj.top/gtlndyopki.html

Ruby: "Hello, #{name}!"
来源：http://hz.bjfxy.top/gtepflayoq.html

C#:   $"Hello, {name}!"
来源：http://hz.ehwqpu.com/gtcwhuffrj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.gzhubu.top/gtoxvvcdkx.html


<!-- 参考信息 -->