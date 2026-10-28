代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://hz.zhongyouzk.top/gtivnxhzvt.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtrvygcjak.html

[U74] PHP：读取环境变量
来源：http://hz.snrcjt.cn/gtsqitvngi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258.top/gteysfkgcw.html

[U75] PHP：依赖注入
来源：http://hz.bjfxy.top/gtzguavncu.html

composer require psr/container
来源：http://hz.xylfe.cn/gthmcyloox.html

[U76] PHP：简单路由
来源：http://hz.iojbl.cn/gtmgqqaqcg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhongyouzk.top/gtqxtyrkpy.html

[U77] PHP：模板渲染
来源：http://hz.yj202588.top/gtkzcsdewk.html

composer require twig/twig
来源：http://hz.ppjwa.cn/gtrgafyipl.html

[U78] PHP：单元测试
来源：http://hz.xylfe.cn/gtszatacyy.html

composer require --dev phpunit/phpunit
来源：http://hz.chenzaomai.com/gtyipyuvsr.html

[U79] PHP：静态分析
来源：http://hz.xuetiantiany.cn/gtxvvqdvxx.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtiqrpjxgm.html

[U80] PHP：代码规范修复
来源：http://hz.gogol.net.cn/gtguohhokm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jlsjyb.cn/gtcxqeyldl.html

[U81] JS：初始化项目
来源：http://hz.ivvv.top/gtnemrsxtz.html

npm init -y;  npm i express
来源：http://hz.c1oappe.top/gtlqxuuduf.html

[U82] JS：package.json 脚本
来源：http://hz.cucudq.cn/gtnmsdphio.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xingfuxueyuan.xyz/gteazeknmh.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtwntqhqkc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gtwlwngucm.html

[U84] JS：CommonJS 写法
来源：http://hz.jianghu66.top/gtwcbsrodi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.vqdsnc.cn/gtscumlrky.html

[U85] JS：可选链
来源：http://hz.daria6918.cn/gtzriicvap.html

a?.b?.c
来源：http://hz.daxiang520.top/gtgprqeyeg.html

[U86] JS：空值合并
来源：http://hz.ydzc1.top/gtynmticnd.html

a ?? b
来源：http://hz.sysykeji.top/gtbuuuklrr.html

[U87] JS：解构默认值
来源：http://hz.pengpengdd.cyou/gtclajrrxh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtfpyezzhe.html

[U88] JS：对象展开合并
来源：http://hz.jlsjyb.cn/gtclsdznog.html

{ ...a, ...b }
来源：http://hz.vqdsnc.cn/gtzuzelvim.html

[U89] JS：数组去重
来源：http://hz.birdmap.top/gtfulcuknb.html

[...new Set(arr)]
来源：http://hz.cqqwz.cn/gthypajned.html

[U90] JS：数字数组排序
来源：http://hz.tian-w.cn/gtnghvufnh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtecqgtzyv.html

[U91] JS：对象键值遍历
来源：http://hz.quarkkingdee.top/gtwqimpjba.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jyoumei.cn/gtpunckwui.html

[U92] JS：深拷贝
来源：http://hz.9152youxi.cn/gtgmexnkmt.html

structuredClone(obj)
来源：http://hz.chenlongwang.top/gtfgramrzm.html

[U93] JS：模板字符串
来源：http://hz.dianchejie.cn/gtaoweplkf.html

`共 ${n} 条`
来源：http://hz.jqgfzy.top/gtdmfmtrio.html

[U94] JS：箭头函数
来源：http://hz.xziqi.cn/gtryzqmqhz.html

const double = x => x * 2;
来源：http://hz.daxiang520.top/gtlowuuavd.html

[U95] JS：Promise 包装
来源：http://hz.tanke756.top/gtqsozjpyf.html

new Promise((resolve, reject) => {})
来源：http://hz.yj20258888.top/gtbqvtyezz.html

[U96] JS：async/await 与异常
来源：http://hz.shanyushiyangtech.top/gtfueenkid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtxoqwfuzz.html

[U97] JS：并发请求
来源：http://hz.jianghu66.top/gtpcysjiqd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gttqbvgojd.html

[U98] JS：fetch 带 JSON
来源：http://hz.zdqjudy.top/gtudcxaxno.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.c1oappe.top/gtrmzhoexq.html

[U99] JS：事件监听
来源：http://hz.yj20258.top/gtmqscukmz.html

el.addEventListener("click", e => {})
来源：http://hz.9152youxi.cn/gthcigpzem.html

[U100] JS：DOM 查询
来源：http://hz.yanxiufei.cn/gtegidumjz.html

document.querySelector(".item")
来源：http://hz.zhongyouzk.top/gthiihkqvf.html

[U101] JS：classList 操作
来源：http://hz.zhongyouzk.top/gtrokkwkof.html

el.classList.toggle("active")
来源：http://hz.tianlin.xyz/gtdndboadv.html

[U102] JS：本地存储
来源：http://hz.xingfuxueyuan.xyz/gtnizzoutz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhengqikj.top/gtzdkqomvi.html

[U103] JS：定时器
来源：http://hz.xinyue.icu/gtscqgvqoy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tianlin.xyz/gtthqpwydb.html

[U104] JS：防抖
来源：http://hz.zhaomingkeji.xyz/gtiwqubcjk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtobjapytx.html

[U105] JS：节流
来源：http://hz.sufxvd.cn/gtnmgmznur.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gttgjmrdps.html

[U106] JS：日期格式化
来源：http://hz.sufxvd.cn/gtccmauwrf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtvgrkuodx.html

[U107] JS：数字千分位
来源：http://hz.gogol.net.cn/gtlkdttlhq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gtrapwuzqk.html

[U108] JS：随机整数
来源：http://hz.yonumen.top/gtowcicrfx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sxryk.cn/gtkydpqwns.html

[U109] JS：数组分组
来源：http://hz.tanke756.top/gttxycmpqt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtwxmhqbtd.html

[U110] JS：数组分块
来源：http://hz.sweek.top/gtlszgnxhf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yvedp.cn/gtrmnnbgxt.html

[U111] JS：对象转 Map
来源：http://hz.xingfuxueyuan.xyz/gtaimgsjwf.html

new Map(Object.entries(obj))
来源：http://hz.fzhhl.top/gtxvlzvgri.html

[U112] JS：字符串补位
来源：http://hz.jlsjyb.cn/gtayymsoyh.html

"7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtazycsygd.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtiasaoofy.html

s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtwrbnygyu.html

[U114] JS：JSON 深比较
来源：http://hz.nanxuanxn.top/gtziheayba.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtfgeyygss.html

[U115] JS：生成 UUID
来源：http://hz.gzhubu.top/gtzrturugz.html

crypto.randomUUID()
来源：http://hz.mhx1999.top/gtqgixvnvt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangdashe.top/gtdgrxhknd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtrttjcrba.html

[U117] JS：单元测试
来源：http://hz.shuidangran.top/gtqxvhyhol.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtbmfhmbts.html

[U118] JS：开发服务器
来源：http://hz.zhoulong.xyz/gtybrnygdg.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtvtskwgxt.html

[U119] JS：生产构建
来源：http://hz.pycfn.com/gthzwmaigr.html

npx vite build
来源：http://hz.aibaodan.cn/gtuckblsoc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nanxuanxn.top/gtynbcpcql.html

import.meta.env.VITE_API_URL
来源：http://hz.smart0.xyz/gtjptppvxg.html

================================================================================
来源：http://hz.birdmap.top/gtfgjmhjts.html

统计汇总
来源：http://hz.zhoulong.xyz/gttrsosnrc.html

================================================================================
来源：http://hz.ppjwa.cn/gtlemgsnzy.html

按语言统计（条）：
来源：http://hz.shanyushiyangkeji.top/gtmpxhhpzc.html

Python ......... 252
来源：http://hz.nwbrower.top/gtubyetihm.html

PHP ............ 252
来源：http://hz.havefunace.top/gtjymdiprn.html

JavaScript ..... 252
来源：http://hz.zhaomingkeji.xyz/gtuxiiyroo.html

TypeScript ..... 212
来源：http://hz.jinyuanbaomall.cn/gtjieshrqx.html

Java ........... 212
来源：http://hz.xziqi.cn/gtcczuqqay.html

Go ............. 212
来源：http://hz.svipenyu.cn/gtodxfosku.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtkgtckzao.html

C# ............. 212
来源：http://hz.aizwys.cn/gtgvyyvmmk.html

C .............. 30
来源：http://hz.birdmap.top/gttornkwvl.html

C++ ............ 30
来源：http://hz.cucudq.cn/gtfmyayexe.html

SQL ............ 90
来源：http://hz.jlsjyb.cn/gtdoxobkpn.html

Bash ........... 80
来源：http://hz.c1oappe.top/gtrlgigrkk.html

Kotlin ......... 15
来源：http://hz.cdnleiting.top/gtqgniavtu.html

Swift .......... 15
来源：http://hz.52xcode.cn/gttbqitwsa.html

Lua ............ 10
来源：http://hz.cucudq.cn/gtqrijpmba.html

Perl ........... 10
来源：http://hz.birdmap.top/gtwjpcougn.html

Scala .......... 10
来源：http://hz.xziqi.cn/gtrnibfdof.html

------------------------------------
来源：http://hz.zhoulong.xyz/gtvhulrldy.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gttzdxzind.html

按章节统计：
来源：http://hz.nwbrower.top/gtosdzpnlq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtrrujaqvk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtrsisutng.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtgrjbyjtm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtuxldsoil.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tian-w.cn/gtpkhwqlga.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtfhbepept.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtxdahwjvi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtzzfayevv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtogjsqokv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gtumtgfvxc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtkyajmyqv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtfpvygfnq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtehvmqgpn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtvskvjysm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.snrcjt.cn/gthyyidxqz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtwmudcneh.html

Q SQL 专题                              90
来源：http://hz.yueranfly.top/gtlfcxcngp.html

R Bash 专题                             80
来源：http://hz.feifeiyinyue.top/gtfxyzdgup.html

S C / C++ 专题                          60
来源：http://hz.mhx1999.top/gtrxmlkczu.html

T 其他语言补充                          60
来源：http://hz.hfpthk.cn/gtcahtxvbi.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtooiqtvgm.html

------------------------------------
来源：http://hz.sweek.top/gtfwuzyxtf.html

合计                                  2106 条
来源：http://hz.pycfn.com/gtcnlnuoop.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtbdvembmc.html

使用提醒
来源：http://hz.ywan-chungtsiang.top/gtmjmrhhwv.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtrmfpipmg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtmtfdnoyc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jlsjyb.cn/gtmrycpcuo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xziqi.cn/gtbpkxbbcm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.quarkkingdee.top/gtxiokgmyx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jqgfzy.top/gtosrfewih.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gteionzulv.html

================================================================================
来源：http://hz.xinyue.icu/gtomqsyjsp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nwbrower.top/gtldzxsbzg.html

Common Programming Examples Cheat Book
来源：http://hz.zhixingplan.top/gtaakmjtuw.html

================================================================================
来源：http://hz.daria6918.cn/gtsgcmdqyv.html

【收录内容】
来源：http://hz.nanxuanxn.top/gtibnvmpnl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhoulong.xyz/gtuywqnsah.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.mhx1999.top/gtlqrcrpsx.html

SQL · Bash · C · C++
来源：http://hz.gogol.net.cn/gtejgmxrry.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cheryme.top/gtcaivnvfg.html

【使用说明】
来源：http://hz.ybcxt.top/gtyeppdxzu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cqqwz.cn/gtmyyzregb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.9152youxi.cn/gtddcmbnzq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtneoaragr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shangyingyoupin.top/gtgrdsddkj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.tianlin.xyz/gtrdehkqmp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yangfankeji.com/gtkyiserre.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.dashuyun.cn/gtkkyykoca.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenzaomai.com/gtclrxyebz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sysykeji.top/gtavewxjdp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gtxrbretgx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xingfuxueyuan.xyz/gtjmhgesod.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.smart0.xyz/gtdfhyqipc.html

【文件统计】
来源：http://hz.bjfxy.top/gtbksflbgv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxuanxn.top/gtvjmcrovo.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtcenxzcji.html

目  录
来源：http://hz.cqqwz.cn/gttfwrhppy.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gtnvsbulop.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.guowangkeji.top/gtmxvtjtuz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gthqlpnwob.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ybcxt.top/gtklwezbae.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tian-w.cn/gtghzpjftq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.bjfxy.top/gtxrzwtyiu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtjviippcq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtkopsuvgc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtfqnymppp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtaignjskp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zdqjudy.top/gtlhxdgprq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtzncsmawk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtywwgbari.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtwkfsbfob.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gteleotcei.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.birdmap.top/gtlzdifqfr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtyoekchcf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gtypjxqdub.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.havefunace.top/gtuqvrawus.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.fzhhl.top/gtjrjpwrjc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtviwkaitv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxinkj.top/gtntxvbgly.html

================================================================================
来源：http://hz.nwbrower.top/gtaevcsrio.html

A. 基础语法与类型
来源：http://hz.yj20258.top/gtiskgsceb.html

================================================================================
来源：http://hz.sufxvd.cn/gteqkqoyku.html

[A01] Hello World
来源：http://hz.chenzaomai.com/gtvtqhdqog.html

Py:   print("Hello, World!")
来源：http://hz.tian-w.cn/gtnmlcwkqp.html

PHP:  echo "Hello, World!";
来源：http://hz.hywenlv.cn/gtoicyzyia.html

JS:   console.log("Hello, World!");
来源：http://hz.daxiang520.top/gteelbmhwj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ivvv.top/gtzpleiwni.html

Java: System.out.println("Hello, World!");
来源：http://hz.pycfn.com/gtezlrbtdw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.meibo888.top/gtfyzubedf.html

Ruby: puts "Hello, World!"
来源：http://hz.aibaodan.cn/gtqasunxty.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenlongwang.top/gtbvfafgxv.html

[A02] 变量声明与赋值
来源：http://hz.nanxinkj.top/gtizypmxlx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.snrcjt.cn/gtewtqqitd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hongshengwenyu.top/gthlazrlwj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtwzfljrrq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gtwfvnliqa.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ivvv.top/gtybfsjsfy.html

Go:   name := "Alex"; age := 20
来源：http://hz.haohaochexian.top/gtjvpmwtzg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daria6918.cn/gtnxqzebat.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gtvfchubhn.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtbkpqlrwu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuanzx.com/gtliitifsc.html

PHP:  const PI = 3.14159;
来源：http://hz.chenlongwang.top/gtqwnhuouj.html

JS:   const PI = 3.14159;
来源：http://hz.smart0.xyz/gttrllyfcj.html

TS:   const PI: number = 3.14159;
来源：http://hz.ybcxt.top/gtondbcprg.html

Java: static final double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtlkaxnxpb.html

Go:   const PI = 3.14159
来源：http://hz.ydzc1.top/gtgnqqzvpl.html

Ruby: PI = 3.14159
来源：http://hz.hammf.cn/gtarwrqwkv.html

C#:   const double PI = 3.14159;
来源：http://hz.yuxming.cn/gttthhpkru.html

[A04] 判断变量类型
来源：http://hz.sufxvd.cn/gtfybuvohg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ybcxt.top/gtgpurqkjy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.feifeiyinyue.top/gtgdmwecdm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yuxming.cn/gtyvvoomaa.html

TS:   typeof x; x instanceof Date
来源：http://hz.nanxinkj.top/gthupfkzgx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.feifeiyinyue.top/gtphfmakgs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xylfe.cn/gtemjdpwdc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shuidangran.top/gtlubxraqz.html

C#:   x.GetType().Name; x is int
来源：http://hz.wangdashe.top/gttruiqgfg.html

[A05] 整数除法与取模
来源：http://hz.xziqi.cn/gtalruhiav.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cqqwz.cn/gtftofwnqd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aizwys.cn/gtbxeqhqaj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtbcooitys.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gttroqgqxl.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhongyouzk.top/gtnjhnlmkr.html

Go:   7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gtxyetafwp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtkzvhkxiz.html

C#:   7 / 2; 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtgaiqiask.html

[A06] 字符串转数字
来源：http://hz.ybcxt.top/gtusqrynno.html

Py:   int("42"); float("3.14")
来源：http://hz.cucudq.cn/gtrjqxhyde.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.havefunace.top/gttoxywnrq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hfpthk.cn/gtnypualdf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtrrgsxhbn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.guowangkeji.top/gtmzqxsmjt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tanke756.top/gtkmyofvjc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.vqdsnc.cn/gthjcpohpt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xuetiantiany.cn/gtpwtnzmld.html

[A07] 数字转字符串
来源：http://hz.shuidangran.top/gthvqznsgi.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtbchiztmk.html

PHP:  (string) 42; strval(42)
来源：http://hz.ybcxt.top/gtslnlttxn.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258.top/gttdjeytpn.html

TS:   String(42)
来源：http://hz.gzhubu.top/gtcbzasfdo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shangyingyoupin.top/gtcnussalw.html

Go:   strconv.Itoa(42)
来源：http://hz.shanyushiyangtech.top/gtmmytghyo.html

Ruby: 42.to_s
来源：http://hz.gzhubu.top/gtevntjcat.html

C#:   42.ToString()
来源：http://hz.iojbl.cn/gttwnlydsr.html

[A08] 取整与四舍五入
来源：http://hz.mhx1999.top/gtqlmnatht.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.tianlin.xyz/gtnwjyatqp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zdqjudy.top/gtsjsndymx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shanyushiyangtech.top/gtkwlgxodp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.9152youxi.cn/gtanpqlvfr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jqgufenzy.top/gtxktobovm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yj20258888.top/gtelvreape.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ybcxt.top/gtwfldqknq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.yj20258.top/gtkjfdonot.html

[A09] 绝对值与最大最小值
来源：http://hz.feifeiyinyue.top/gtuevsdrgm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.wangdashe.top/gtsnsyegct.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ivvv.top/gtwyrvffjv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nwbrower.top/gtchbidbgo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnqzz.top/gtfubcodiv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.0kj1m.cn/gtpbxewndj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.tianlin.xyz/gtnupwrdfw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jlsjyb.cn/gtoubilngb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.iojbl.cn/gtdrkgooik.html

[A10] 生成随机数
来源：http://hz.jlsjyb.cn/gtyqywcfia.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ydjk.org.cn/gtkvaifcvv.html

PHP:  random_int(1, 100);
来源：http://hz.zhijiandao.cn/gtszzvjpyv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daxiang520.top/gtxzymciwx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jinqigufen.top/gtvfxommiu.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gogol.net.cn/gthbelnnnj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhixingplan.top/gttzcjgdnw.html

Ruby: rand(1..100)
来源：http://hz.daria6918.cn/gtyzxmkwpr.html

C#:   new Random().Next(1, 101)
来源：http://hz.52xcode.cn/gtwuyyrrjx.html

[A11] 条件表达式（三元）
来源：http://hz.hfpthk.cn/gtznkpphmi.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.gotoacloud.top/gttheqejpi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtaqfijriz.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtxdjjqpxv.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.daria6918.cn/gtzvmrsium.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gthayscqxo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.zhixingplan.top/gtnknqnzpl.html


<!-- 参考信息 -->