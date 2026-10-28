代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hz.zhengqikj.top/gtrsahewqe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtqtosmjxp.html

[U70] PHP：PDO 事务
来源：http://hz.ydjk.org.cn/gtiiueemew.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ybcxt.top/gtnkdegnpo.html

[U71] PHP：抛出异常
来源：http://hz.9152youxi.cn/gtujhdgpcf.html

throw new RuntimeException("失败", 500);
来源：http://hz.pycfn.com/gtywywlrjb.html

[U72] PHP：写错误日志
来源：http://hz.yj202588.top/gtgatuocwh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtygdolshc.html

[U73] PHP：读取 ini 配置
来源：http://hz.xinyue.icu/gtpajrzode.html

parse_ini_file("config.ini", true)
来源：http://hz.zhongyouzk.top/gtvujwmeds.html

[U74] PHP：读取环境变量
来源：http://hz.0kj1m.cn/gtiyjpwnfh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.pycfn.com/gtllvawjat.html

[U75] PHP：依赖注入
来源：http://hz.wangshuangyany.cn/gtxkhspqdr.html

composer require psr/container
来源：http://hz.0kj1m.cn/gttdeovarn.html

[U76] PHP：简单路由
来源：http://hz.shangyingyoupin.top/gtiaaffhws.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cdnleiting.top/gtklolmflx.html

[U77] PHP：模板渲染
来源：http://hz.zhaomingkeji.xyz/gtrlpyskzi.html

composer require twig/twig
来源：http://hz.zhiwuduotai.top/gtpbkvutbq.html

[U78] PHP：单元测试
来源：http://hz.jianghu66.top/gtctxkxpft.html

composer require --dev phpunit/phpunit
来源：http://hz.xuanzx.com/gtqoczpcwq.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangtech.top/gtvkcezbwx.html

composer require --dev phpstan/phpstan
来源：http://hz.yonumen.top/gtjrrfavfr.html

[U80] PHP：代码规范修复
来源：http://hz.gaohongyu789.top/gtapnbwpbh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nwbrower.top/gtbfjubxec.html

[U81] JS：初始化项目
来源：http://hz.daxiang520.top/gtkqutlbyj.html

npm init -y;  npm i express
来源：http://hz.yonumen.top/gtismzovls.html

[U82] JS：package.json 脚本
来源：http://hz.jinghuilouyu.cn/gtolkphjsh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.redwolf501.top/gtpffsjpqu.html

[U83] JS：ES Module 导入导出
来源：http://hz.fengsongda.top/gtbosehhao.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.haohaochexian.top/gtctobneev.html

[U84] JS：CommonJS 写法
来源：http://hz.snrcjt.cn/gtlifdfknm.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtdtjoabhm.html

[U85] JS：可选链
来源：http://hz.aizwys.cn/gtlncjvwoa.html

a?.b?.c
来源：http://hz.ydzc1.top/gtlplhcmub.html

[U86] JS：空值合并
来源：http://hz.xziqi.cn/gtnfzxkbvv.html

a ?? b
来源：http://hz.andypj.xyz/gtyyxxbnae.html

[U87] JS：解构默认值
来源：http://hz.yj202588.top/gtvbfpzeey.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinyuanbaomall.cn/gtcjzmxnwd.html

[U88] JS：对象展开合并
来源：http://hz.chenlongwang.top/gtdatlwqng.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtgoopzzzt.html

[U89] JS：数组去重
来源：http://hz.ehwqpu.com/gtkzoabhrz.html

[...new Set(arr)]
来源：http://hz.zhijiandao.cn/gttjegtnts.html

[U90] JS：数字数组排序
来源：http://hz.yuanzhike.top/gtowojacfm.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtnslcafij.html

[U91] JS：对象键值遍历
来源：http://hz.nanxuanxn.top/gtyhpqhbix.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigfzy.top/gtlcxwyvxp.html

[U92] JS：深拷贝
来源：http://hz.9152youxi.cn/gtdtljxueg.html

structuredClone(obj)
来源：http://hz.yangfankeji.com/gtfjrornkm.html

[U93] JS：模板字符串
来源：http://hz.sysykeji.top/gtjqppfjcj.html

`共 ${n} 条`
来源：http://hz.shuidangran.top/gtsxxfdcri.html

[U94] JS：箭头函数
来源：http://hz.zhijiandao.cn/gtywxqashl.html

const double = x => x * 2;
来源：http://hz.c1oappe.top/gteithxdou.html

[U95] JS：Promise 包装
来源：http://hz.havefunace.top/gtjoubjizn.html

new Promise((resolve, reject) => {})
来源：http://hz.yanxiufei.cn/gtefognhvy.html

[U96] JS：async/await 与异常
来源：http://hz.gogol.net.cn/gtzgaxbsjo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtjwobymku.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtdweojnth.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtccrbuwdt.html

[U98] JS：fetch 带 JSON
来源：http://hz.xinyue.icu/gtpmtimtsp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shangyingyoupin.top/gtclkhaciu.html

[U99] JS：事件监听
来源：http://hz.sxryk.cn/gtnxpxicgj.html

el.addEventListener("click", e => {})
来源：http://hz.shangyingyoupin.top/gthribbhen.html

[U100] JS：DOM 查询
来源：http://hz.snrcjt.cn/gtsadhmcpx.html

document.querySelector(".item")
来源：http://hz.shzxlz.cn/gtwdnmmohe.html

[U101] JS：classList 操作
来源：http://hz.yonumen.top/gtaeevmmlm.html

el.classList.toggle("active")
来源：http://hz.xingfuxueyuan.xyz/gtbfjgwfnl.html

[U102] JS：本地存储
来源：http://hz.hfpthk.cn/gtxpfpquqn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtsskenzpe.html

[U103] JS：定时器
来源：http://hz.ivvv.top/gtmdvqsicx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hongshengwenyu.top/gtxrcmdtoj.html

[U104] JS：防抖
来源：http://hz.jinghuilouyu.cn/gtcytzylwd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtujrmngpo.html

[U105] JS：节流
来源：http://hz.gaohongyu789.top/gtigqzgqlo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtjxmsbtwy.html

[U106] JS：日期格式化
来源：http://hz.52xcode.cn/gtardrjgcx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtouuvkdtc.html

[U107] JS：数字千分位
来源：http://hz.chenlongwang.top/gtmfvxlglb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtwusdthcw.html

[U108] JS：随机整数
来源：http://hz.xingfuxueyuan.xyz/gtwjuscxti.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yueranfly.top/gtmnueyojx.html

[U109] JS：数组分组
来源：http://hz.jyoumei.cn/gthgvslozu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtafpkuavb.html

[U110] JS：数组分块
来源：http://hz.wangdashe.top/gtrnwjclfe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhijiandao.cn/gtnaocwggz.html

[U111] JS：对象转 Map
来源：http://hz.nanxuanxn.top/gtbigufvxx.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtwgzlqflx.html

[U112] JS：字符串补位
来源：http://hz.sysykeji.top/gtrbrcbwsl.html

"7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtmqiauwww.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gttaguoupe.html

s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtbwewcuxx.html

[U114] JS：JSON 深比较
来源：http://hz.havefunace.top/gtnnhnmbav.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtmgrwqiqz.html

[U115] JS：生成 UUID
来源：http://hz.shuidangran.top/gtgvitkold.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtxxpgawzt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.daria6918.cn/gtwlqqakbz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.wangshuangyany.cn/gtabgxxler.html

[U117] JS：单元测试
来源：http://hz.daria6918.cn/gttzvxaect.html

npm i -D vitest;  npx vitest
来源：http://hz.aibaodan.cn/gtshpipyoi.html

[U118] JS：开发服务器
来源：http://hz.andypj.xyz/gtuliclgbk.html

npm i -D vite;  npx vite
来源：http://hz.gaohongyu789.top/gtvlkwezcu.html

[U119] JS：生产构建
来源：http://hz.andypj.xyz/gtawsfnmrv.html

npx vite build
来源：http://hz.nwbrower.top/gtjhipqgru.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258.top/gttmuubcfv.html

import.meta.env.VITE_API_URL
来源：http://hz.dashuyun.cn/gtumnczriw.html

================================================================================
来源：http://hz.zhengqikj.top/gtvmkuabjt.html

统计汇总
来源：http://hz.birdmap.top/gtvqxzmfkf.html

================================================================================
来源：http://hz.hywenlv.cn/gtygwnurhb.html

按语言统计（条）：
来源：http://hz.gogol.net.cn/gtqcucjyzk.html

Python ......... 252
来源：http://hz.mhx1999.top/gtfgogyima.html

PHP ............ 252
来源：http://hz.hammf.cn/gtuevohqea.html

JavaScript ..... 252
来源：http://hz.iojbl.cn/gtsgfcxgly.html

TypeScript ..... 212
来源：http://hz.yvedp.cn/gtvjciowdj.html

Java ........... 212
来源：http://hz.jinqigufen.top/gtbudkyafq.html

Go ............. 212
来源：http://hz.snrcjt.cn/gtvxdfvlbp.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gtupwslanz.html

C# ............. 212
来源：http://hz.gaohongyu789.top/gtaffjbrpp.html

C .............. 30
来源：http://hz.jinghuilouyu.cn/gthdkdeetq.html

C++ ............ 30
来源：http://hz.jinyuanbaomall.cn/gtiamqvtoa.html

SQL ............ 90
来源：http://hz.birdmap.top/gtbqhuatjf.html

Bash ........... 80
来源：http://hz.hysaishi.cn/gtvoqbjlle.html

Kotlin ......... 15
来源：http://hz.chenjidiqi.icu/gteakgltzm.html

Swift .......... 15
来源：http://hz.vqdsnc.cn/gtggybfafn.html

Lua ............ 10
来源：http://hz.hammf.cn/gtjzgovhtf.html

Perl ........... 10
来源：http://hz.yj20258888.top/gtsegtcdhg.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gtscelpstf.html

------------------------------------
来源：http://hz.birdmap.top/gtkzsxyahc.html

合计 ........... 2106 条
来源：http://hz.ybcxt.top/gthflobsgo.html

按章节统计：
来源：http://hz.havefunace.top/gtfyddbrde.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gtlmkeyzup.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtyhzfpumu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtormjxsgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtzgxegjvt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tianlin.xyz/gtrwjnpuuf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.bjfxy.top/gteonvwreu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtnrnttxiz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtuxdljdoc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtvwqdelwu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtbtspunwb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gttmxsqyyy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtrsaauvpu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtyfspecyi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.iojbl.cn/gtbenapbbp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hammf.cn/gtmektpxqh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtuxvreegg.html

Q SQL 专题                              90
来源：http://hz.xylfe.cn/gtvdumvqzc.html

R Bash 专题                             80
来源：http://hz.hywenlv.cn/gtbnhfdsmb.html

S C / C++ 专题                          60
来源：http://hz.ybcxt.top/gthgvaydew.html

T 其他语言补充                          60
来源：http://hz.quarkkingdee.top/gtfitnjhgg.html

U 高频实用片段                         120
来源：http://hz.svipenyu.cn/gtvrwwcexa.html

------------------------------------
来源：http://hz.cqqwz.cn/gthwfgwhjr.html

合计                                  2106 条
来源：http://hz.wangshuangyany.cn/gtxdfvaixg.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtjuxeayiy.html

使用提醒
来源：http://hz.jlsjyb.cn/gtmbvsfecf.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtsahidxqp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guowangkeji.top/gtxgcndgce.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhengqikj.top/gtcawzgqar.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gtifryweny.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gaohongyu789.top/gtuguuzdou.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhaomingkeji.xyz/gtzdgwobln.html

—— 文件结束 ——
来源：http://hz.bjfxy.top/gtxajufieb.html

================================================================================
来源：http://hz.sufxvd.cn/gtjyotcptn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxuanxn.top/gtpppizyhg.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gtdqxxmfqw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrywqdqgf.html

【收录内容】
来源：http://hz.zhixingplan.top/gtbvaqwfht.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daria6918.cn/gtfcfiztje.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yueranfly.top/gtyxwhpcvm.html

SQL · Bash · C · C++
来源：http://hz.9152youxi.cn/gtygjicqtb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangdashe.top/gttjgmaeuw.html

【使用说明】
来源：http://hz.shanyushiyangkeji.top/gtwwwsjhzn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhoulong.xyz/gtshpapiqg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jlsjyb.cn/gtmitoeqjd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nwbrower.top/gtwxptlbmh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tanke756.top/gtdqrzpxec.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.aizwys.cn/gtiddkqvze.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinyuanbaomall.cn/gtxhoexjgc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.smart0.xyz/gtroifzhlg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.bjfxy.top/gtjdizwyhc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cheryme.top/gtmyacxjsp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.svipenyu.cn/gtcrpdrhlt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgufenzy.top/gtmutjfahk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yj202588.top/gtyzmocqfx.html

【文件统计】
来源：http://hz.meibo888.top/gtyrjvbovr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gotoacloud.top/gthpurkffv.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtjtvsunoc.html

目  录
来源：http://hz.smart0.xyz/gtcreoazjv.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtjkyyiixp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gtstpzsbfz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtddjuurip.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gthsywstyp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhoulong.xyz/gtgaoqxxmf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zdqjudy.top/gtrzksuijt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tanke756.top/gtcexqwxab.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhixingplan.top/gtchumjzvh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cashguo.top/gtydtpwxbl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtbteemjqq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtebvotbww.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtftrjccpa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtqmwzzlcr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtxyyxtzcv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ywan-chungtsiang.top/gtfplbdxjo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtzentyznt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtjwpyazhl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gogol.net.cn/gtoodjptcp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhiwuduotai.top/gtagdmduaz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ppjwa.cn/gtufpygjgl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtzgrarzua.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gotoacloud.top/gtglcoziik.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnxmgivzp.html

A. 基础语法与类型
来源：http://hz.zhijiandao.cn/gtkbrvdpla.html

================================================================================
来源：http://hz.andypj.xyz/gtcsinkjlk.html

[A01] Hello World
来源：http://hz.0kj1m.cn/gthkrtzzlc.html

Py:   print("Hello, World!")
来源：http://hz.yvedp.cn/gtapvulcqr.html

PHP:  echo "Hello, World!";
来源：http://hz.hysaishi.cn/gtcydinzcx.html

JS:   console.log("Hello, World!");
来源：http://hz.ybcxt.top/gtoevjpfqf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hammf.cn/gtaljvvkhf.html

Java: System.out.println("Hello, World!");
来源：http://hz.ydjk.org.cn/gtypanamvg.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.smart0.xyz/gtcfkoyhic.html

Ruby: puts "Hello, World!"
来源：http://hz.xinyue.icu/gtqoxzhbvu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jqgfzy.top/gtabigsrci.html

[A02] 变量声明与赋值
来源：http://hz.jqgfzy.top/gtkiyjtlgq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gotoacloud.top/gtumtdznsl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yonumen.top/gtszjivkgv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zdqjudy.top/gtdanzsxai.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pengpengdd.cyou/gtssbgeczu.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinyuanbaomall.cn/gtlbeixlca.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenjidiqi.icu/gteghqfplm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtawfmitzp.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtjbyqzflx.html

[A03] 常量定义
来源：http://hz.cheryme.top/gtzyzouxab.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gtpquafttt.html

PHP:  const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtdhkopvlg.html

JS:   const PI = 3.14159;
来源：http://hz.smart0.xyz/gtauhbpzbo.html

TS:   const PI: number = 3.14159;
来源：http://hz.quarkkingdee.top/gtzbtgwuff.html

Java: static final double PI = 3.14159;
来源：http://hz.52xcode.cn/gtvjsqywst.html

Go:   const PI = 3.14159
来源：http://hz.guannengcc.top/gtufcnmrte.html

Ruby: PI = 3.14159
来源：http://hz.hongshengwenyu.top/gtohoniclk.html

C#:   const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gteaxvwtle.html

[A04] 判断变量类型
来源：http://hz.haohaochexian.top/gtxspjdxaw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xinyue.icu/gtiycmljcp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.svipenyu.cn/gtnkcbtluc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.9152youxi.cn/gtbocylgsj.html

TS:   typeof x; x instanceof Date
来源：http://hz.c1oappe.top/gtndntbuiy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.guannengcc.top/gtigafdhuc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnxiangtu.top/gtfbtlmpgo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxinkj.top/gtkapmwagz.html

C#:   x.GetType().Name; x is int
来源：http://hz.tanke756.top/gtctifdzhw.html

[A05] 整数除法与取模
来源：http://hz.guannengcc.top/gtafyzpovy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.c1oappe.top/gtgnwcnaeq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtlvwoqpaj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cheryme.top/gtvfsihzqu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nwbrower.top/gtktnulszd.html

Java: 7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtbaueuyoa.html

Go:   7 / 2; 7 % 2
来源：http://hz.tanke756.top/gthllxrptj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.aibaodan.cn/gtafgcklsd.html

C#:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtwddlrzqd.html

[A06] 字符串转数字
来源：http://hz.ivvv.top/gtavmnurex.html

Py:   int("42"); float("3.14")
来源：http://hz.xylfe.cn/gtdsqjjcef.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hywenlv.cn/gtfuifvfnb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.smart0.xyz/gtkabcsyyo.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.wangdashe.top/gtsvahfnnu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenzaomai.com/gtxppullyp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.kuanghao11.cn/gtqxyjydlg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.chenjidiqi.icu/gtubijsbgj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jiagoushi.top/gtphnbkirx.html

[A07] 数字转字符串
来源：http://hz.cheryme.top/gtuhxnesiw.html

Py:   str(42)
来源：http://hz.zycfv.cn/gtnmjolxkh.html

PHP:  (string) 42; strval(42)
来源：http://hz.wangshuangyany.cn/gtlmzzihmh.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtszrknszo.html

TS:   String(42)
来源：http://hz.jinqigfzy.top/gtapkkgfuv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.guowangkeji.top/gtfrfzdpcz.html

Go:   strconv.Itoa(42)
来源：http://hz.guowangkeji.top/gtonzwquqf.html

Ruby: 42.to_s
来源：http://hz.aizwys.cn/gtchwluguj.html

C#:   42.ToString()
来源：http://hz.chenzaomai.com/gtvvsagooj.html

[A08] 取整与四舍五入
来源：http://hz.guowangkeji.top/gtjnccsfag.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.chenjidiqi.icu/gttvpwdjbw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.cqqwz.cn/gtdkhtedhh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.guannengcc.top/gtbgrwwjiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.daxiang520.top/gtqbrkmgtf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yangfankeji.com/gtndbmdooe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.chenzaomai.com/gtyvfcjjsk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yongpay.top/gtqohoymcl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yongpay.top/gtjafijhon.html

[A09] 绝对值与最大最小值
来源：http://hz.tian-w.cn/gtovvzbtlz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258.top/gthpuvvrck.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hnqzz.top/gtydolquhs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.gogol.net.cn/gthmueoyyt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yuanzhike.top/gtffzxhpht.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtrfhhyuiv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yonumen.top/gtnjqbftku.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.sysykeji.top/gtbkkyixlz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.kuanghao11.cn/gtznaxnhea.html

[A10] 生成随机数
来源：http://hz.hammf.cn/gtgwcugddc.html

Py:   import random; random.randint(1, 100)
来源：http://hz.0kj1m.cn/gttowujuwg.html

PHP:  random_int(1, 100);
来源：http://hz.jqgfzy.top/gtdjavdgtn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xuanzx.com/gtsfqogkrg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gtyurhynvm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinghuilouyu.cn/gtjjytptcq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinqigufen.top/gtxnvrchym.html

Ruby: rand(1..100)
来源：http://hz.cdnleiting.top/gtgvaultni.html


<!-- 参考信息 -->