代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.yvedp.cn/gtefzdgthb.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenzaomai.com/gtjobrihbj.html

[U72] PHP：写错误日志
来源：http://hz.yangfankeji.com/gttqxemxoa.html

error_log("失败: " . $e->getMessage());
来源：http://hz.iojbl.cn/gtecmguusr.html

[U73] PHP：读取 ini 配置
来源：http://hz.gaohongyu789.top/gtyhkcvixs.html

parse_ini_file("config.ini", true)
来源：http://hz.jinyuanbaomall.cn/gtjduhmexm.html

[U74] PHP：读取环境变量
来源：http://hz.zhongyouzk.top/gtivfilkab.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fzhhl.top/gtidcljbbt.html

[U75] PHP：依赖注入
来源：http://hz.shzxlz.cn/gtoxlkreqx.html

composer require psr/container
来源：http://hz.ydjk.org.cn/gtktogzumy.html

[U76] PHP：简单路由
来源：http://hz.aizwys.cn/gtrizwdxop.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtewnknuro.html

[U77] PHP：模板渲染
来源：http://hz.dianchejie.cn/gtqglwfccr.html

composer require twig/twig
来源：http://hz.ppjwa.cn/gtegpfzrcc.html

[U78] PHP：单元测试
来源：http://hz.quarkkingdee.top/gtfhodritj.html

composer require --dev phpunit/phpunit
来源：http://hz.dianchejie.cn/gtertbvjnb.html

[U79] PHP：静态分析
来源：http://hz.sweek.top/gtoeejkciu.html

composer require --dev phpstan/phpstan
来源：http://hz.shzxlz.cn/gtlbbwxowb.html

[U80] PHP：代码规范修复
来源：http://hz.guowangkeji.top/gtjbportol.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.vqdsnc.cn/gtbgqokivd.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtyxifpmds.html

npm init -y;  npm i express
来源：http://hz.andypj.xyz/gtmnrqouxz.html

[U82] JS：package.json 脚本
来源：http://hz.zhengqikj.top/gtqdxspbjx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.9152youxi.cn/gtdfwjtyjd.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhixingplan.top/gtaettktrh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gogol.net.cn/gtmpfrkozq.html

[U84] JS：CommonJS 写法
来源：http://hz.bjfxy.top/gtkycusvwa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tianlin.xyz/gthqvhkebs.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtdxjjfarl.html

a?.b?.c
来源：http://hz.sufxvd.cn/gtpjtyphre.html

[U86] JS：空值合并
来源：http://hz.jyoumei.cn/gtolcfwble.html

a ?? b
来源：http://hz.nanxinkj.top/gtotvwqppw.html

[U87] JS：解构默认值
来源：http://hz.cdnleiting.top/gtnixaxdud.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gotoacloud.top/gtolratmik.html

[U88] JS：对象展开合并
来源：http://hz.wangshuangyany.cn/gtftmajpwu.html

{ ...a, ...b }
来源：http://hz.jinyuanbaomall.cn/gtxaifyiie.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtykenggoe.html

[...new Set(arr)]
来源：http://hz.shzxlz.cn/gtocauvisc.html

[U90] JS：数字数组排序
来源：http://hz.hywenlv.cn/gtxqexxvny.html

[...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtpigxewfb.html

[U91] JS：对象键值遍历
来源：http://hz.hfpthk.cn/gtvrmvwwwy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hammf.cn/gtlwoncfmp.html

[U92] JS：深拷贝
来源：http://hz.havefunace.top/gtactnvamj.html

structuredClone(obj)
来源：http://hz.chenzaomai.com/gtffgshops.html

[U93] JS：模板字符串
来源：http://hz.jianghu66.top/gtdvaykgof.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtuamiijho.html

[U94] JS：箭头函数
来源：http://hz.yvedp.cn/gtzusaiang.html

const double = x => x * 2;
来源：http://hz.cashguo.top/gtjiivqkoz.html

[U95] JS：Promise 包装
来源：http://hz.ydjk.org.cn/gttzfbalez.html

new Promise((resolve, reject) => {})
来源：http://hz.jyoumei.cn/gtmgaweecq.html

[U96] JS：async/await 与异常
来源：http://hz.hywenlv.cn/gtllvcqoub.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtotvchrsp.html

[U97] JS：并发请求
来源：http://hz.yvedp.cn/gtohufspwv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtvzlatjjo.html

[U98] JS：fetch 带 JSON
来源：http://hz.kuanghao11.cn/gtqafeqehs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuetiantiany.cn/gtmgfswljn.html

[U99] JS：事件监听
来源：http://hz.jqgfzy.top/gtouqcxwoj.html

el.addEventListener("click", e => {})
来源：http://hz.haohaochexian.top/gteqijiwvk.html

[U100] JS：DOM 查询
来源：http://hz.gzhubu.top/gtonrvwigv.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtvcjnpmyk.html

[U101] JS：classList 操作
来源：http://hz.hysaishi.cn/gtckrxgbiz.html

el.classList.toggle("active")
来源：http://hz.jinqigfzy.top/gtmsdbgodj.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtizfrukih.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guannengcc.top/gtocalmomu.html

[U103] JS：定时器
来源：http://hz.gotoacloud.top/gtrqvmgall.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.316326.xyz/gtdimujhpq.html

[U104] JS：防抖
来源：http://hz.tanke756.top/gtsurvmhca.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gteywthhqq.html

[U105] JS：节流
来源：http://hz.fzhhl.top/gtsoygcpxx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.birdmap.top/gtrkkyzyxx.html

[U106] JS：日期格式化
来源：http://hz.yonumen.top/gtkylnfkqv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuanzx.com/gtkmztsutd.html

[U107] JS：数字千分位
来源：http://hz.dianchejie.cn/gtgkjauugs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gogol.net.cn/gthbiiaefu.html

[U108] JS：随机整数
来源：http://hz.chenlongwang.top/gtkhetqevt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtglfdfgfb.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtzvsxnsrz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtezsdwxln.html

[U110] JS：数组分块
来源：http://hz.hnxiangtu.top/gtyzwxdkcq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dashuyun.cn/gtcusmedqd.html

[U111] JS：对象转 Map
来源：http://hz.quarkkingdee.top/gtcrnqqzrn.html

new Map(Object.entries(obj))
来源：http://hz.yonumen.top/gtahwnuolk.html

[U112] JS：字符串补位
来源：http://hz.snrcjt.cn/gtfneyxynd.html

"7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtkgqscacu.html

[U113] JS：正则替换全部
来源：http://hz.ivvv.top/gticswqacp.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gttubbuuuu.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtnzukmzdk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtsejxlvpc.html

[U115] JS：生成 UUID
来源：http://hz.xuetiantiany.cn/gtdlpwzugf.html

crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtzoimsmou.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtioqquzau.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gogol.net.cn/gtuejnngmq.html

[U117] JS：单元测试
来源：http://hz.yj20258888.top/gteawclsuw.html

npm i -D vitest;  npx vitest
来源：http://hz.ppjwa.cn/gtanomrouw.html

[U118] JS：开发服务器
来源：http://hz.hongshengwenyu.top/gtuzisoomj.html

npm i -D vite;  npx vite
来源：http://hz.hywenlv.cn/gthvmyykts.html

[U119] JS：生产构建
来源：http://hz.tianlin.xyz/gteeczokij.html

npx vite build
来源：http://hz.xingfuxueyuan.xyz/gtqzfxogqo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.pycfn.com/gtkebqvtvf.html

import.meta.env.VITE_API_URL
来源：http://hz.nanxuanxn.top/gthfjtuczd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnspptoni.html

统计汇总
来源：http://hz.sweek.top/gttunahgaf.html

================================================================================
来源：http://hz.hywenlv.cn/gtnawayaif.html

按语言统计（条）：
来源：http://hz.feifeiyinyue.top/gteaiiohnb.html

Python ......... 252
来源：http://hz.yuxming.cn/gtkmjjbouo.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtmjyofrjn.html

JavaScript ..... 252
来源：http://hz.zhijiandao.cn/gtfgnfwabm.html

TypeScript ..... 212
来源：http://hz.yongpay.top/gttnvrgecw.html

Java ........... 212
来源：http://hz.guowangkeji.top/gtdiuqnokp.html

Go ............. 212
来源：http://hz.tianlin.xyz/gtrqukgwif.html

Ruby ........... 212
来源：http://hz.yonumen.top/gtejckpfxk.html

C# ............. 212
来源：http://hz.quarkkingdee.top/gttwevswwh.html

C .............. 30
来源：http://hz.shuidangran.top/gtvsayoepg.html

C++ ............ 30
来源：http://hz.birdmap.top/gtahepjrha.html

SQL ............ 90
来源：http://hz.0kj1m.cn/gtouqcmzdb.html

Bash ........... 80
来源：http://hz.jiagoushi.top/gtkwtsuxmx.html

Kotlin ......... 15
来源：http://hz.yuanzhike.top/gtuvaytprh.html

Swift .......... 15
来源：http://hz.tianlin.xyz/gthyfwcchv.html

Lua ............ 10
来源：http://hz.ivvv.top/gtmofshomu.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtmqnbfhed.html

Scala .......... 10
来源：http://hz.nanxuanxn.top/gtbnkxueoq.html

------------------------------------
来源：http://hz.sxryk.cn/gtljeidhot.html

合计 ........... 2106 条
来源：http://hz.bjfxy.top/gtoomqgjzh.html

按章节统计：
来源：http://hz.jiagoushi.top/gtophnvkkr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhongyouzk.top/gtsklhncjk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtzczfnqtd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtjucmhguz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtalyyxbpo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj202588.top/gtuwtvmesr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtzozhvbja.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.316326.xyz/gtwdfspimo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuxming.cn/gtdzyweafh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.meibo888.top/gtqzwdadlj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtoeijlurq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtjugnoeao.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtfuwetwiz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtuezvkchj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.mhx1999.top/gtgrmvoekj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ivvv.top/gtagylxjmi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtvbcgywra.html

Q SQL 专题                              90
来源：http://hz.yj202588.top/gtmszuefxb.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtfdtrhvix.html

S C / C++ 专题                          60
来源：http://hz.guannengcc.top/gtdwtddoxv.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gttbjvitcz.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gtzmyycgng.html

------------------------------------
来源：http://hz.hysaishi.cn/gtrooefdem.html

合计                                  2106 条
来源：http://hz.xylfe.cn/gtlwbzxpxp.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtkkwsxrjx.html

使用提醒
来源：http://hz.yuxming.cn/gthfwzzefi.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gtlqyvccdf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.svipenyu.cn/gtoefdmznq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tianlin.xyz/gtawxiabtj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ydjk.org.cn/gttsislpiz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhixingplan.top/gtdkkgiwno.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.nanxuanxn.top/gtgzyqxphh.html

—— 文件结束 ——
来源：http://hz.tanke756.top/gtaszznuch.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcbsuhngs.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtuguuibrr.html

Common Programming Examples Cheat Book
来源：http://hz.snrcjt.cn/gtmhxzvssq.html

================================================================================
来源：http://hz.xinyue.icu/gtvaabroco.html

【收录内容】
来源：http://hz.zhiwuduotai.top/gtqwwneccq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shzxlz.cn/gtnpctkatr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hongshengwenyu.top/gtxswduedy.html

SQL · Bash · C · C++
来源：http://hz.sysykeji.top/gturtjweci.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtiavauupx.html

【使用说明】
来源：http://hz.yj20258888.top/gtxpexrikr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yj202588.top/gtocnowwif.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtcnebbyha.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinqigufen.top/gtuckrtswq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jiagoushi.top/gtzamgioni.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.cashguo.top/gtmxdocslp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.aibaodan.cn/gtrjmffqgt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.snrcjt.cn/gtdnlotadz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj202588.top/gtzlkxmnlx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shuidangran.top/gtojtzhyvg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jinghuilouyu.cn/gtwzzsfhke.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtdzvdphsh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinqigfzy.top/gtctvzcxso.html

【文件统计】
来源：http://hz.zycfv.cn/gtqvyhrgky.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jinghuilouyu.cn/gtlbyskapb.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtvvfjrlee.html

目  录
来源：http://hz.sysykeji.top/gtftbbcghu.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtzztrdanr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gttngxxahn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtfyendxer.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtbovstfev.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.bjfxy.top/gtagmdfaok.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zhaomingkeji.xyz/gtntajqalu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gtuvdzdjwm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtzhzwdmiu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtzxcgpncx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtjbyoudiu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtqccwifru.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtjhkmluea.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtpismyjyk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtskekzmsr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtgomljxqc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.vqdsnc.cn/gtfjmqstoq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtoukknnwo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fengsongda.top/gtbuqtgdzh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhengqikj.top/gtydvobeyx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.pengpengdd.cyou/gtqncfyosw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtcpkcctnz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhaomingkeji.xyz/gtpgpjufge.html

================================================================================
来源：http://hz.nwbrower.top/gtbboxblit.html

A. 基础语法与类型
来源：http://hz.shangyingyoupin.top/gtrppsrzed.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthsnadzyl.html

[A01] Hello World
来源：http://hz.meibo888.top/gtdnyivbhg.html

Py:   print("Hello, World!")
来源：http://hz.jlsjyb.cn/gttrwqraar.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigfzy.top/gtdvspnxem.html

JS:   console.log("Hello, World!");
来源：http://hz.fzhhl.top/gtksdffumr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yongpay.top/gtebzkutnq.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuxming.cn/gtvfhjtqls.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtutomdxjo.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtjcvycjbl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jqgfzy.top/gthgrkbnde.html

[A02] 变量声明与赋值
来源：http://hz.9152youxi.cn/gtnprbbrxb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yvedp.cn/gtbpngawov.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.chenzaomai.com/gtjkmeiehd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yongpay.top/gtstminxef.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gthdknwwmw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtcgiljwte.html

Go:   name := "Alex"; age := 20
来源：http://hz.aibaodan.cn/gtrdqcxnkv.html

Ruby: name = "Alex"; age = 20
来源：http://hz.aizwys.cn/gtrhbqmfuh.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.redwolf501.top/gtkcautbzf.html

[A03] 常量定义
来源：http://hz.jinyuanbaomall.cn/gtzuqkpqbz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj202588.top/gtrxjvjiej.html

PHP:  const PI = 3.14159;
来源：http://hz.ppjwa.cn/gtyifjsips.html

JS:   const PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtcoyqzdcc.html

TS:   const PI: number = 3.14159;
来源：http://hz.jianghu66.top/gtecorxrbj.html

Java: static final double PI = 3.14159;
来源：http://hz.birdmap.top/gtewochjjv.html

Go:   const PI = 3.14159
来源：http://hz.gogol.net.cn/gtmaltguuf.html

Ruby: PI = 3.14159
来源：http://hz.zhixingplan.top/gtyhiwjwhb.html

C#:   const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtcuquomij.html

[A04] 判断变量类型
来源：http://hz.xziqi.cn/gtxzrlpksf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zdqjudy.top/gtybbjukwh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhengqikj.top/gtfraewgdf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.fengsongda.top/gtgflzqzse.html

TS:   typeof x; x instanceof Date
来源：http://hz.ehwqpu.com/gttjvkagyg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinqigufen.top/gtwnrcsjde.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.316326.xyz/gthaepzoos.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.guannengcc.top/gtjngjocem.html

C#:   x.GetType().Name; x is int
来源：http://hz.dashuyun.cn/gtkydebrqr.html

[A05] 整数除法与取模
来源：http://hz.yuanzhike.top/gthzximxdh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.pycfn.com/gtjvucatjc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hywenlv.cn/gthiwyrvwu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.316326.xyz/gtcvnyhpay.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnxiangtu.top/gtzfwkcful.html

Java: 7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtzgimhcem.html

Go:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtypwkdmio.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.aibaodan.cn/gtoiweyemn.html

C#:   7 / 2; 7 % 2
来源：http://hz.fengsongda.top/gtiywycnvy.html

[A06] 字符串转数字
来源：http://hz.zdqjudy.top/gttwsokddz.html

Py:   int("42"); float("3.14")
来源：http://hz.bjfxy.top/gtxedrgrgu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jiagoushi.top/gtbdhxqhwy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aizwys.cn/gtbozrdnju.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shuidangran.top/gtnqdxkhkz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.aizwys.cn/gtpnprcxte.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.sxryk.cn/gtjitiuwck.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.nanxuanxn.top/gtzwcpamdw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangdashe.top/gtnheukxot.html

[A07] 数字转字符串
来源：http://hz.fzhhl.top/gtlbrbcnjg.html

Py:   str(42)
来源：http://hz.havefunace.top/gtnmoukfxt.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhengqikj.top/gtmbjmzsfy.html

JS:   String(42); (42).toString()
来源：http://hz.gogol.net.cn/gtijymvvsg.html

TS:   String(42)
来源：http://hz.yj202588.top/gtkweslakj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.daria6918.cn/gtmpftrlpf.html

Go:   strconv.Itoa(42)
来源：http://hz.zdqjudy.top/gtzytxzahq.html

Ruby: 42.to_s
来源：http://hz.pengpengdd.cyou/gtcgbttvpb.html

C#:   42.ToString()
来源：http://hz.tanke756.top/gtmezabquw.html

[A08] 取整与四舍五入
来源：http://hz.meibo888.top/gtrsvpmxyd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ppjwa.cn/gtlbfwcret.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ppjwa.cn/gtsruwrdkc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhoulong.xyz/gtsewzqsmt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yj202588.top/gtmyegtzdm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtesgpjjpf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.snrcjt.cn/gtskbuwlho.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ppjwa.cn/gtvsunijac.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yongpay.top/gtstddvefm.html

[A09] 绝对值与最大最小值
来源：http://hz.xylfe.cn/gtkuwfwgzz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.meibo888.top/gtroffrxqu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.birdmap.top/gtdeswmgnl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.daria6918.cn/gtxhuqlmiw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.316326.xyz/gtptrotjmt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xziqi.cn/gtuqlkkzcp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cashguo.top/gtrslasnpq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.zhoulong.xyz/gtawsjajin.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ehwqpu.com/gtncwotmnm.html

[A10] 生成随机数
来源：http://hz.jyoumei.cn/gtkdmokmbn.html

Py:   import random; random.randint(1, 100)
来源：http://hz.bjfxy.top/gtptckkpbw.html

PHP:  random_int(1, 100);
来源：http://hz.xziqi.cn/gtxlodtggg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yangfankeji.com/gtfgsfeeae.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.0kj1m.cn/gtcvbduxqv.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ywan-chungtsiang.top/gtjpwmcedm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yongpay.top/gtdricxihe.html

Ruby: rand(1..100)
来源：http://hz.yj20258.top/gtucfgsidy.html

C#:   new Random().Next(1, 101)
来源：http://hz.hammf.cn/gtgggceyvm.html

[A11] 条件表达式（三元）
来源：http://hz.c1oappe.top/gtqcatxgpv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cdnleiting.top/gtgiccmgiz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtxugzrbpj.html


<!-- 参考信息 -->