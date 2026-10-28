代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.smart0.xyz/gtgxbktfzc.html

throw new RuntimeException("失败", 500);
来源：http://hz.svipenyu.cn/gtqmszyqni.html

[U72] PHP：写错误日志
来源：http://hz.yangfankeji.com/gtljdbxdmb.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hywenlv.cn/gtucygikwb.html

[U73] PHP：读取 ini 配置
来源：http://hz.bjfxy.top/gtgrnddzkn.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gtobgtjwnk.html

[U74] PHP：读取环境变量
来源：http://hz.52xcode.cn/gtmcvwrbpl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenzaomai.com/gtwcdctpku.html

[U75] PHP：依赖注入
来源：http://hz.zhijiandao.cn/gtcbzcucjo.html

composer require psr/container
来源：http://hz.dianchejie.cn/gthkqkxwqe.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtbecabsbw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cheryme.top/gtokdyyjkb.html

[U77] PHP：模板渲染
来源：http://hz.shuidangran.top/gtcxnoknst.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gtzxjznqsr.html

[U78] PHP：单元测试
来源：http://hz.ybcxt.top/gthlldswpo.html

composer require --dev phpunit/phpunit
来源：http://hz.ywan-chungtsiang.top/gtvdxllimg.html

[U79] PHP：静态分析
来源：http://hz.yongpay.top/gtdzdnsiij.html

composer require --dev phpstan/phpstan
来源：http://hz.tanke756.top/gtqndxfeun.html

[U80] PHP：代码规范修复
来源：http://hz.tanke756.top/gttxcjkcpn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yj202588.top/gttiasunnf.html

[U81] JS：初始化项目
来源：http://hz.quarkkingdee.top/gtjnceylkf.html

npm init -y;  npm i express
来源：http://hz.yj20258.top/gthbliasoo.html

[U82] JS：package.json 脚本
来源：http://hz.cheryme.top/gtwziiddim.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fzhhl.top/gtohojeihb.html

[U83] JS：ES Module 导入导出
来源：http://hz.havefunace.top/gtkcgnqyxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xinyue.icu/gttthfbjzp.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtgsooxhoz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yanxiufei.cn/gtlknqgzsl.html

[U85] JS：可选链
来源：http://hz.hysaishi.cn/gteltcrnri.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtlopxljql.html

[U86] JS：空值合并
来源：http://hz.sxryk.cn/gtexyxzvwn.html

a ?? b
来源：http://hz.nanxinkj.top/gthzhuxolj.html

[U87] JS：解构默认值
来源：http://hz.chenzaomai.com/gtiuguyazg.html

const { a = 1, b = 2 } = obj;
来源：http://hz.mhx1999.top/gtouhutjsw.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtzizcwhnl.html

{ ...a, ...b }
来源：http://hz.zhijiandao.cn/gtfgwtdord.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gtegccdoyb.html

[...new Set(arr)]
来源：http://hz.jiagoushi.top/gtwcdclatn.html

[U90] JS：数字数组排序
来源：http://hz.hysaishi.cn/gtaxhikkla.html

[...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gthgphseir.html

[U91] JS：对象键值遍历
来源：http://hz.shangyingyoupin.top/gthhcmnyfx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yanxiufei.cn/gtcpelbdaf.html

[U92] JS：深拷贝
来源：http://hz.chenzaomai.com/gtvrfnsgpy.html

structuredClone(obj)
来源：http://hz.birdmap.top/gtypierdfn.html

[U93] JS：模板字符串
来源：http://hz.nanxuanxn.top/gtcrlubdsc.html

`共 ${n} 条`
来源：http://hz.yj20258.top/gtmgydiedu.html

[U94] JS：箭头函数
来源：http://hz.fzhhl.top/gtcqoxeyhx.html

const double = x => x * 2;
来源：http://hz.snrcjt.cn/gtgemzugvz.html

[U95] JS：Promise 包装
来源：http://hz.jiagoushi.top/gtnmkwxheo.html

new Promise((resolve, reject) => {})
来源：http://hz.gzhubu.top/gtqkgotcac.html

[U96] JS：async/await 与异常
来源：http://hz.jinghuilouyu.cn/gtmeoztgxl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtebyxbhwy.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangkeji.top/gtijmxwspl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtcpbxwnfg.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gtrwnighcx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hongshengwenyu.top/gtbbpxvpum.html

[U99] JS：事件监听
来源：http://hz.cheryme.top/gtqxztwncx.html

el.addEventListener("click", e => {})
来源：http://hz.cucudq.cn/gtznwiudxa.html

[U100] JS：DOM 查询
来源：http://hz.zhaomingkeji.xyz/gtltgyfmxn.html

document.querySelector(".item")
来源：http://hz.zhengqikj.top/gtlxptmacl.html

[U101] JS：classList 操作
来源：http://hz.birdmap.top/gtgwvsbyvc.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtnubeoacf.html

[U102] JS：本地存储
来源：http://hz.tian-w.cn/gtxumayyan.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtljelpfoz.html

[U103] JS：定时器
来源：http://hz.bjfxy.top/gtkyikctpb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.bjfxy.top/gtmskxmhwh.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gtzjkotmoi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtypruspck.html

[U105] JS：节流
来源：http://hz.c1oappe.top/gtoklxaiki.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jyoumei.cn/gtuxiygrvt.html

[U106] JS：日期格式化
来源：http://hz.cheryme.top/gtwjdjlvav.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nwbrower.top/gtqzvbsbwm.html

[U107] JS：数字千分位
来源：http://hz.jyoumei.cn/gtkafdjmjd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtmhslmfkm.html

[U108] JS：随机整数
来源：http://hz.iojbl.cn/gtapceghkq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangkeji.top/gtuxwonsua.html

[U109] JS：数组分组
来源：http://hz.jlsjyb.cn/gtlcdsqvan.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtnqkdgyor.html

[U110] JS：数组分块
来源：http://hz.hfpthk.cn/gtxfskdtvp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.mhx1999.top/gtcwapmmhf.html

[U111] JS：对象转 Map
来源：http://hz.sufxvd.cn/gtymhtfxzh.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtuefsppjt.html

[U112] JS：字符串补位
来源：http://hz.ppjwa.cn/gtptpcpvqs.html

"7".padStart(3, "0")
来源：http://hz.tanke756.top/gtctoctymo.html

[U113] JS：正则替换全部
来源：http://hz.xuanzx.com/gtufgedxvk.html

s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtmjrfyqam.html

[U114] JS：JSON 深比较
来源：http://hz.jyoumei.cn/gtbmcqzdmn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtglktmeck.html

[U115] JS：生成 UUID
来源：http://hz.cashguo.top/gtaemvbcpf.html

crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtvcqexpww.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yueranfly.top/gtdwszpfje.html

/** @param {string} name */ function f(name) {}
来源：http://hz.fzhhl.top/gtbkfnvugh.html

[U117] JS：单元测试
来源：http://hz.chenlongwang.top/gtgbskugbu.html

npm i -D vitest;  npx vitest
来源：http://hz.daxiang520.top/gtiztskgfm.html

[U118] JS：开发服务器
来源：http://hz.ivvv.top/gttcxcdcjq.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtqsxwcgbz.html

[U119] JS：生产构建
来源：http://hz.xuanzx.com/gtdmybyrtm.html

npx vite build
来源：http://hz.guowangkeji.top/gtucymlltm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhengqikj.top/gtlfjpyoog.html

import.meta.env.VITE_API_URL
来源：http://hz.hongshengwenyu.top/gttfpbzmcq.html

================================================================================
来源：http://hz.svipenyu.cn/gtjuubmqul.html

统计汇总
来源：http://hz.c1oappe.top/gtububcoio.html

================================================================================
来源：http://hz.c1oappe.top/gtrnfmbaku.html

按语言统计（条）：
来源：http://hz.snrcjt.cn/gtshethnmj.html

Python ......... 252
来源：http://hz.hywenlv.cn/gtzizzabeg.html

PHP ............ 252
来源：http://hz.yj20258.top/gtbqthdsyk.html

JavaScript ..... 252
来源：http://hz.nanxuanxn.top/gtqubhzsum.html

TypeScript ..... 212
来源：http://hz.haohaochexian.top/gtlwhbnaqd.html

Java ........... 212
来源：http://hz.nanxinkj.top/gtdeyurdlm.html

Go ............. 212
来源：http://hz.nwbrower.top/gtphgeclaz.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtsyqjzyik.html

C# ............. 212
来源：http://hz.xylfe.cn/gtqsoggzfk.html

C .............. 30
来源：http://hz.jinghuilouyu.cn/gtfpgiwcaz.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtkuolexqn.html

SQL ............ 90
来源：http://hz.jiagoushi.top/gtbnysuheb.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtlzgsnhmp.html

Kotlin ......... 15
来源：http://hz.hysaishi.cn/gttdwzkgsw.html

Swift .......... 15
来源：http://hz.mhx1999.top/gtvdzadzvg.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtjxrlnozd.html

Perl ........... 10
来源：http://hz.tian-w.cn/gtabkxtsqx.html

Scala .......... 10
来源：http://hz.jinqigfzy.top/gtkiqdaavi.html

------------------------------------
来源：http://hz.shangyingyoupin.top/gttcehnonx.html

合计 ........... 2106 条
来源：http://hz.nanxuanxn.top/gthjpfgxmm.html

按章节统计：
来源：http://hz.dianchejie.cn/gtjnvaqezu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yonumen.top/gtrrkhhnkq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtnclyzhpi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtplqnafpe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtyyhjfeci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.wangshuangyany.cn/gtblsbieci.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtdounjppc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtmthxvcwe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gtipqemyot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtxggqpwow.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.quarkkingdee.top/gtvhnktfot.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtodvdywpd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gthvqwkooe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtwkmawqcs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtwqnkwjwu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yangfankeji.com/gtbvxuwzwe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtmhvdrpfc.html

Q SQL 专题                              90
来源：http://hz.yanxiufei.cn/gtujvzncmw.html

R Bash 专题                             80
来源：http://hz.bjfxy.top/gttnmyucwf.html

S C / C++ 专题                          60
来源：http://hz.daria6918.cn/gtrkfyzkbh.html

T 其他语言补充                          60
来源：http://hz.hysaishi.cn/gtwxoometv.html

U 高频实用片段                         120
来源：http://hz.hywenlv.cn/gtvigifzfp.html

------------------------------------
来源：http://hz.jinqigufen.top/gtalelqlyr.html

合计                                  2106 条
来源：http://hz.xinyue.icu/gtoeukdljn.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtuwehlxjb.html

使用提醒
来源：http://hz.nanxuanxn.top/gtofirvelg.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gttfjvvzwo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.52xcode.cn/gthpiyvujv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenlongwang.top/gtsmstczyv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yvedp.cn/gtytzzggoi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.pengpengdd.cyou/gtaqibgbzl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.meibo888.top/gtkvfejkeu.html

—— 文件结束 ——
来源：http://hz.yj202588.top/gtkbbvawfa.html

================================================================================
来源：http://hz.nanxinkj.top/gtgchyjmfd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.snrcjt.cn/gttjdlowlw.html

Common Programming Examples Cheat Book
来源：http://hz.yangfankeji.com/gtwdnljdbb.html

================================================================================
来源：http://hz.52xcode.cn/gtfptltxko.html

【收录内容】
来源：http://hz.quarkkingdee.top/gtsmbviboj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cdnleiting.top/gtfopdjjbz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.havefunace.top/gtknlicxom.html

SQL · Bash · C · C++
来源：http://hz.kuanghao11.cn/gtvahoxfde.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dashuyun.cn/gtpiedxula.html

【使用说明】
来源：http://hz.ydjk.org.cn/gtihjjdfup.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xuanzx.com/gtpvlwhtui.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yueranfly.top/gtcygszmhe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhoulong.xyz/gtdtoxegjc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.9152youxi.cn/gtzwjkgesm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.tanke756.top/gtdmyitnks.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhoulong.xyz/gtkscupqwp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhengqikj.top/gtjczxqvgg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fzhhl.top/gtgyjdbnzh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yongpay.top/gtjbbxbczq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj202588.top/gtsysywipv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.guannengcc.top/gteztvvapk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.chenjidiqi.icu/gtdibhvrwi.html

【文件统计】
来源：http://hz.yonumen.top/gtwiefhaix.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sufxvd.cn/gttenrtwrw.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtzzgblgmq.html

目  录
来源：http://hz.pycfn.com/gtkqbddusu.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258.top/gtjiaqrhug.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.guannengcc.top/gtfakkylqg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtvowbzwkr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gthjnaorqx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.smart0.xyz/gtfdiwveoi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hywenlv.cn/gtmixshola.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.smart0.xyz/gtxttypwaa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.dashuyun.cn/gteichcwcj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtabqfigrh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtgqshtfwr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cheryme.top/gtniaixdgm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtwtyghutg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtvkxheijv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtbnskwuhs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.daxiang520.top/gtkyocsrns.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.svipenyu.cn/gtiqrwecci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtcrodzgdo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.andypj.xyz/gtpsxjbepy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtcyiqmsnf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ppjwa.cn/gtdhtuzwma.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yongpay.top/gtvgezzqzt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtmhhvejnq.html

================================================================================
来源：http://hz.iojbl.cn/gtjbnhyrtz.html

A. 基础语法与类型
来源：http://hz.zhijiandao.cn/gtnzrharpv.html

================================================================================
来源：http://hz.sysykeji.top/gtdtuinytw.html

[A01] Hello World
来源：http://hz.ybcxt.top/gtnjeezapu.html

Py:   print("Hello, World!")
来源：http://hz.guowangkeji.top/gtxyvxrunu.html

PHP:  echo "Hello, World!";
来源：http://hz.shuidangran.top/gthixqkogl.html

JS:   console.log("Hello, World!");
来源：http://hz.nanxuanxn.top/gtnvhclbri.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhengqikj.top/gtknegugrl.html

Java: System.out.println("Hello, World!");
来源：http://hz.shzxlz.cn/gtajvduxtb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.nwbrower.top/gtbumeklzr.html

Ruby: puts "Hello, World!"
来源：http://hz.zdqjudy.top/gtuxclinph.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.snrcjt.cn/gttzjfkfuv.html

[A02] 变量声明与赋值
来源：http://hz.gaohongyu789.top/gttkkihtmx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.redwolf501.top/gtkkxbwder.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuxming.cn/gtyspwdhth.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinqigfzy.top/gtlhapwjkd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.wangdashe.top/gtapgwfxhl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtwkhdahvz.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangdashe.top/gtmolaltyc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daxiang520.top/gtequbnscp.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtxmfwnucz.html

[A03] 常量定义
来源：http://hz.jianghu66.top/gtygpyjdqa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ybcxt.top/gtqfhbvtnq.html

PHP:  const PI = 3.14159;
来源：http://hz.hfpthk.cn/gtuqitpbrx.html

JS:   const PI = 3.14159;
来源：http://hz.jinqigufen.top/gtkkazguwl.html

TS:   const PI: number = 3.14159;
来源：http://hz.jiagoushi.top/gtphpyfbbw.html

Java: static final double PI = 3.14159;
来源：http://hz.tanke756.top/gtwzdismwn.html

Go:   const PI = 3.14159
来源：http://hz.fzhhl.top/gtdxpsfhpd.html

Ruby: PI = 3.14159
来源：http://hz.hysaishi.cn/gtwmvcqjti.html

C#:   const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtlsapkqsm.html

[A04] 判断变量类型
来源：http://hz.redwolf501.top/gthkvjncfl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangshuangyany.cn/gtgzzqfmtd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xinyue.icu/gtznmtchyd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhengqikj.top/gthbqwoawd.html

TS:   typeof x; x instanceof Date
来源：http://hz.shuidangran.top/gtsecsngxw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gtjmlmeewl.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tanke756.top/gtwpiovlzq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuanzhike.top/gtvpguqmwy.html

C#:   x.GetType().Name; x is int
来源：http://hz.zdqjudy.top/gtlasyepjn.html

[A05] 整数除法与取模
来源：http://hz.vqdsnc.cn/gtfpaahcpy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxuanxn.top/gtzlhawuuq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yonumen.top/gtzfcvsxpt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258888.top/gtoytuhudz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.dashuyun.cn/gtkduykubs.html

Java: 7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtnwyzhapi.html

Go:   7 / 2; 7 % 2
来源：http://hz.sufxvd.cn/gtiruwbfca.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gtymmhyauf.html

C#:   7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtojjslows.html

[A06] 字符串转数字
来源：http://hz.ivvv.top/gtmiobdzke.html

Py:   int("42"); float("3.14")
来源：http://hz.hfpthk.cn/gtpmtsuuzt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.iojbl.cn/gtbccdkffu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenjidiqi.icu/gttusjhplc.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.hnxiangtu.top/gtnfbewvpd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.birdmap.top/gtmfpucyqq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ywan-chungtsiang.top/gtenxdyrdd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yueranfly.top/gtaejsuqwm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.quarkkingdee.top/gtsaahmtlq.html

[A07] 数字转字符串
来源：http://hz.gaohongyu789.top/gttblwkixw.html

Py:   str(42)
来源：http://hz.hongshengwenyu.top/gtfoungtey.html

PHP:  (string) 42; strval(42)
来源：http://hz.gaohongyu789.top/gtbkhtzxge.html

JS:   String(42); (42).toString()
来源：http://hz.jiagoushi.top/gtwjybipnb.html

TS:   String(42)
来源：http://hz.jinqigufen.top/gtsiltgewj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.cheryme.top/gtvtjptalk.html

Go:   strconv.Itoa(42)
来源：http://hz.9152youxi.cn/gtkpmdlqfv.html

Ruby: 42.to_s
来源：http://hz.cucudq.cn/gtsdmptgww.html

C#:   42.ToString()
来源：http://hz.pengpengdd.cyou/gtltmwtwbz.html

[A08] 取整与四舍五入
来源：http://hz.cucudq.cn/gttbkrdzqt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtkjrasbbr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cashguo.top/gtciiihnqs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhijiandao.cn/gtysbzbnly.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cashguo.top/gtnhvhaifu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtikxitadi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.guowangkeji.top/gtesqmswyw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yuxming.cn/gttsgssdlk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.tianlin.xyz/gtntyjobxn.html

[A09] 绝对值与最大最小值
来源：http://hz.shanyushiyangkeji.top/gtfscyghjf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yangfankeji.com/gtlwykeoit.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtigapbljp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xziqi.cn/gtxrfvhkcg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shuidangran.top/gtadhhlhid.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jlsjyb.cn/gtunopxgpf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinyuanbaomall.cn/gtqpbtrdqx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cashguo.top/gtrdzfwmgy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ppjwa.cn/gtdjxydnyq.html

[A10] 生成随机数
来源：http://hz.cashguo.top/gtbxzqepie.html

Py:   import random; random.randint(1, 100)
来源：http://hz.dianchejie.cn/gtunxtownq.html

PHP:  random_int(1, 100);
来源：http://hz.mhx1999.top/gtuunvsbqr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shangyingyoupin.top/gtonspvnxq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.iojbl.cn/gtqjroecaa.html

Java: new Random().nextInt(100) + 1
来源：http://hz.svipenyu.cn/gtvenugxpv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.smart0.xyz/gtyqwiiekg.html

Ruby: rand(1..100)
来源：http://hz.yonumen.top/gtkppmyggg.html

C#:   new Random().Next(1, 101)
来源：http://hz.cheryme.top/gtciussamw.html

[A11] 条件表达式（三元）
来源：http://hz.hongshengwenyu.top/gtnimzobsy.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xinyue.icu/gtlnbqvnxx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtukmhuxwk.html


<!-- 参考信息 -->