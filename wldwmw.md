代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://hz.snrcjt.cn/gtrflozooi.html

parse_ini_file("config.ini", true)
来源：http://hz.aibaodan.cn/gtqyxpxahs.html

[U74] PHP：读取环境变量
来源：http://hz.shzxlz.cn/gtxqdoxlbq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tanke756.top/gtocyuyfin.html

[U75] PHP：依赖注入
来源：http://hz.chenzaomai.com/gtketgdzsp.html

composer require psr/container
来源：http://hz.jqgfzy.top/gtdmgttfpz.html

[U76] PHP：简单路由
来源：http://hz.cdnleiting.top/gtyvchtpsn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhengqikj.top/gtxyukdiat.html

[U77] PHP：模板渲染
来源：http://hz.shangyingyoupin.top/gtqwnwxwfk.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gtadgidevo.html

[U78] PHP：单元测试
来源：http://hz.tianlin.xyz/gtgpktzadg.html

composer require --dev phpunit/phpunit
来源：http://hz.cqqwz.cn/gtqpttrpty.html

[U79] PHP：静态分析
来源：http://hz.zhoulong.xyz/gtxltajnrj.html

composer require --dev phpstan/phpstan
来源：http://hz.ivvv.top/gtuebgmqof.html

[U80] PHP：代码规范修复
来源：http://hz.xuetiantiany.cn/gtalqbyulv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yj20258888.top/gtjgxecdvb.html

[U81] JS：初始化项目
来源：http://hz.smart0.xyz/gtqituglgb.html

npm init -y;  npm i express
来源：http://hz.jlsjyb.cn/gtddsgnlag.html

[U82] JS：package.json 脚本
来源：http://hz.shuidangran.top/gtqtvhadtc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.vqdsnc.cn/gtjsgjzacj.html

[U83] JS：ES Module 导入导出
来源：http://hz.hammf.cn/gtxpnwulfu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtuleoxqlc.html

[U84] JS：CommonJS 写法
来源：http://hz.yangfankeji.com/gtsobnbrcy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tanke756.top/gtryrwwnrj.html

[U85] JS：可选链
来源：http://hz.shanyushiyangtech.top/gthnteemrc.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtggqohelc.html

[U86] JS：空值合并
来源：http://hz.jiagoushi.top/gtmhtjkfdb.html

a ?? b
来源：http://hz.yueranfly.top/gtdmtscopu.html

[U87] JS：解构默认值
来源：http://hz.yj202588.top/gtmmrqkmkz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hongshengwenyu.top/gtgzzhoxrq.html

[U88] JS：对象展开合并
来源：http://hz.shangyingyoupin.top/gtfimelcec.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gtlorcxvls.html

[U89] JS：数组去重
来源：http://hz.jinghuilouyu.cn/gtlurikptg.html

[...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtchxlmfah.html

[U90] JS：数字数组排序
来源：http://hz.sweek.top/gtbxwgwwal.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtcnrzanuw.html

[U91] JS：对象键值遍历
来源：http://hz.nwbrower.top/gthxbikhfz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj202588.top/gtenglcpdu.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtxpktenlk.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtqiejiqro.html

[U93] JS：模板字符串
来源：http://hz.chenlongwang.top/gtbbofptjk.html

`共 ${n} 条`
来源：http://hz.ivvv.top/gtibobobpx.html

[U94] JS：箭头函数
来源：http://hz.ybcxt.top/gtxxmhgrvz.html

const double = x => x * 2;
来源：http://hz.ydzc1.top/gtxvdwdvkv.html

[U95] JS：Promise 包装
来源：http://hz.fzhhl.top/gtxjbiphkp.html

new Promise((resolve, reject) => {})
来源：http://hz.yuanzhike.top/gtpbupltpz.html

[U96] JS：async/await 与异常
来源：http://hz.chenlongwang.top/gtqzenuymi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtaxaezodw.html

[U97] JS：并发请求
来源：http://hz.yangfankeji.com/gtvksfdfrb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtrgadyqvv.html

[U98] JS：fetch 带 JSON
来源：http://hz.chenzaomai.com/gtpbklvsga.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydzc1.top/gtflrfetwq.html

[U99] JS：事件监听
来源：http://hz.andypj.xyz/gtalfgxcku.html

el.addEventListener("click", e => {})
来源：http://hz.jinqigfzy.top/gtklyewnbh.html

[U100] JS：DOM 查询
来源：http://hz.redwolf501.top/gtrwpqnkhm.html

document.querySelector(".item")
来源：http://hz.jqgfzy.top/gtaqgwjgjj.html

[U101] JS：classList 操作
来源：http://hz.shanyushiyangkeji.top/gtxzqftcwd.html

el.classList.toggle("active")
来源：http://hz.yj202588.top/gttjxwpjgs.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtpcjsoczy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinghuilouyu.cn/gtmpvrsjvp.html

[U103] JS：定时器
来源：http://hz.guannengcc.top/gtazzohunu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinghuilouyu.cn/gtyjtlkuhm.html

[U104] JS：防抖
来源：http://hz.fzhhl.top/gthdosedxy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtotdltjdk.html

[U105] JS：节流
来源：http://hz.yanxiufei.cn/gtlqmgrhnr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinghuilouyu.cn/gtnfnsxngi.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gthdvefrwp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinyuanbaomall.cn/gtyhbwecnh.html

[U107] JS：数字千分位
来源：http://hz.ppjwa.cn/gthrknbzan.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gtjsypnqyk.html

[U108] JS：随机整数
来源：http://hz.ybcxt.top/gtbrrmkhki.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtqturtqnt.html

[U109] JS：数组分组
来源：http://hz.cheryme.top/gtntdstmjw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtrmaugdsp.html

[U110] JS：数组分块
来源：http://hz.9152youxi.cn/gtpiomwjot.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.316326.xyz/gttcnfbecv.html

[U111] JS：对象转 Map
来源：http://hz.yueranfly.top/gtghgpvmce.html

new Map(Object.entries(obj))
来源：http://hz.vqdsnc.cn/gtiwiptnyf.html

[U112] JS：字符串补位
来源：http://hz.cheryme.top/gtihtbwvqa.html

"7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtpvlaekye.html

[U113] JS：正则替换全部
来源：http://hz.xylfe.cn/gthtqbjwny.html

s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtauhyudet.html

[U114] JS：JSON 深比较
来源：http://hz.chenlongwang.top/gtiqzvuovl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtvadugsof.html

[U115] JS：生成 UUID
来源：http://hz.cqqwz.cn/gtizhxcfsk.html

crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtwajdmffl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.birdmap.top/gtqrffyupv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhoulong.xyz/gtzfkhqhvc.html

[U117] JS：单元测试
来源：http://hz.zhijiandao.cn/gtmwvzgans.html

npm i -D vitest;  npx vitest
来源：http://hz.yj202588.top/gtjncfqlep.html

[U118] JS：开发服务器
来源：http://hz.dashuyun.cn/gtzkguajma.html

npm i -D vite;  npx vite
来源：http://hz.havefunace.top/gtfscczddo.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtvdknefoe.html

npx vite build
来源：http://hz.daria6918.cn/gtacqsknxb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gthwznqnjt.html

import.meta.env.VITE_API_URL
来源：http://hz.zdqjudy.top/gtrmzztobo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpyzfprju.html

统计汇总
来源：http://hz.daria6918.cn/gtqqvzrssw.html

================================================================================
来源：http://hz.sxryk.cn/gtgpsikkav.html

按语言统计（条）：
来源：http://hz.ydzc1.top/gtpsvbtcft.html

Python ......... 252
来源：http://hz.yj20258888.top/gtkkrsilhr.html

PHP ............ 252
来源：http://hz.c1oappe.top/gtbwyewpqr.html

JavaScript ..... 252
来源：http://hz.pycfn.com/gthoucvvum.html

TypeScript ..... 212
来源：http://hz.hfpthk.cn/gtvulhytzj.html

Java ........... 212
来源：http://hz.redwolf501.top/gtdobaiith.html

Go ............. 212
来源：http://hz.nanxinkj.top/gtnaluisfa.html

Ruby ........... 212
来源：http://hz.dashuyun.cn/gtwvgzgggr.html

C# ............. 212
来源：http://hz.jinghuilouyu.cn/gtemzvtnjz.html

C .............. 30
来源：http://hz.smart0.xyz/gtuiswmrsj.html

C++ ............ 30
来源：http://hz.cucudq.cn/gtpaxssglu.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gtfzwohsnp.html

Bash ........... 80
来源：http://hz.daria6918.cn/gtgoecnfbu.html

Kotlin ......... 15
来源：http://hz.jqgufenzy.top/gtwrrrlmgu.html

Swift .......... 15
来源：http://hz.ywan-chungtsiang.top/gtvuhrboqu.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtnpamssej.html

Perl ........... 10
来源：http://hz.pycfn.com/gtmlcjdqxm.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtidmmrmda.html

------------------------------------
来源：http://hz.chenlongwang.top/gtptkoerrb.html

合计 ........... 2106 条
来源：http://hz.kuanghao11.cn/gtykhfnyqf.html

按章节统计：
来源：http://hz.hongshengwenyu.top/gteupymciw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtatjwnmpk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtwxiwssga.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtsjnsepyg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gtfggcycse.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hysaishi.cn/gtfeaxpefn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.daxiang520.top/gtawajptyq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtsmlfrqet.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gttosqbhue.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gttitwyqwn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangtech.top/gtmyaurcve.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtylppmxnj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gttyqxxumq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtmworpkay.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtvtxwzggi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.haohaochexian.top/gtzogqgrir.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gttxmaigke.html

Q SQL 专题                              90
来源：http://hz.xinyue.icu/gtuxspgduh.html

R Bash 专题                             80
来源：http://hz.kuanghao11.cn/gtqewdddrm.html

S C / C++ 专题                          60
来源：http://hz.cashguo.top/gtwicltgau.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtmtpkgdxi.html

U 高频实用片段                         120
来源：http://hz.shzxlz.cn/gtpgelztqo.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gtdkoriojc.html

合计                                  2106 条
来源：http://hz.wangdashe.top/gtbzzkqlml.html

--------------------------------------------------------------------------------
来源：http://hz.fengsongda.top/gtflsfsmov.html

使用提醒
来源：http://hz.shzxlz.cn/gtocyghbai.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gthkqkrzmm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gthxkngywh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guowangkeji.top/gttcmylspa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ehwqpu.com/gtyoczfrlz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.dianchejie.cn/gtjfnnrvgm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ppjwa.cn/gtklfvwmvp.html

—— 文件结束 ——
来源：http://hz.jqgufenzy.top/gtbzneysoe.html

================================================================================
来源：http://hz.xziqi.cn/gttcxqojka.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gthdwrwtbc.html

Common Programming Examples Cheat Book
来源：http://hz.vqdsnc.cn/gtftgrkkws.html

================================================================================
来源：http://hz.hammf.cn/gtnajgztid.html

【收录内容】
来源：http://hz.sxryk.cn/gtqrvhdlxr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yongpay.top/gtvopnufih.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nwbrower.top/gtmthtlyxw.html

SQL · Bash · C · C++
来源：http://hz.fengsongda.top/gtepabxqao.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenzaomai.com/gtxltvbfpu.html

【使用说明】
来源：http://hz.chenzaomai.com/gtxnlkybsf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangshuangyany.cn/gtnrblugwv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guannengcc.top/gtqepybfjh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yuxming.cn/gtihcggqlf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gtcyagtoht.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.quarkkingdee.top/gtgugxkpic.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xuetiantiany.cn/gtrvyezeoh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ivvv.top/gttabahpou.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yongpay.top/gtugjfckgs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shuidangran.top/gtqrlesomy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jyoumei.cn/gtpcwdvouk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pengpengdd.cyou/gtgejmbmcw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sweek.top/gtebvuroll.html

【文件统计】
来源：http://hz.zhiwuduotai.top/gtdotfeiaw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jiagoushi.top/gtawkmkppf.html

--------------------------------------------------------------------------------
来源：http://hz.pengpengdd.cyou/gtwzhtqycc.html

目  录
来源：http://hz.hnxiangtu.top/gtpkzygysl.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtgkdqzkws.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gtzkjusoqh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtewlifvyl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtuitihusv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.guannengcc.top/gtixaytnur.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.guannengcc.top/gtdxjoetmn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.feifeiyinyue.top/gtvyxjipjb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtatplwvjm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tanke756.top/gttwywuvli.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtjsicnyti.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gtzzobfylb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.dashuyun.cn/gtbohcfaob.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtfdcrtzov.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtrfafmrpm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtpfhnxdjc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ehwqpu.com/gtqliytglp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yanxiufei.cn/gtbdjidyqk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yonumen.top/gtanceroum.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangkeji.top/gtyhiromzm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tanke756.top/gtcqafpdof.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtriuclqiv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtewgvglol.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthdagxlut.html

A. 基础语法与类型
来源：http://hz.xuetiantiany.cn/gttybevduy.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrqzcjdqb.html

[A01] Hello World
来源：http://hz.fzhhl.top/gtnhtvteka.html

Py:   print("Hello, World!")
来源：http://hz.yj202588.top/gtelscqxiu.html

PHP:  echo "Hello, World!";
来源：http://hz.jinqigfzy.top/gtkzjygkyf.html

JS:   console.log("Hello, World!");
来源：http://hz.cdnleiting.top/gtbrbqswrl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.birdmap.top/gtnscwkwbk.html

Java: System.out.println("Hello, World!");
来源：http://hz.andypj.xyz/gtrtnoplst.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jiagoushi.top/gtuknuuyoh.html

Ruby: puts "Hello, World!"
来源：http://hz.jlsjyb.cn/gteyfydezg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenzaomai.com/gtnaaczxpn.html

[A02] 变量声明与赋值
来源：http://hz.jinyuanbaomall.cn/gtdtpnzoge.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ehwqpu.com/gtbesnbenl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.dashuyun.cn/gtypsirklt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.quarkkingdee.top/gtoveekjth.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jlsjyb.cn/gtvygtfeia.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtedvillne.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtywhegtmu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hnxiangtu.top/gtxbswotby.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtclxljfoh.html

[A03] 常量定义
来源：http://hz.ybcxt.top/gtglqtiqxj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuanzhike.top/gtjufkpxtf.html

PHP:  const PI = 3.14159;
来源：http://hz.jinqigufen.top/gtehkyenmm.html

JS:   const PI = 3.14159;
来源：http://hz.xinyue.icu/gtlifqhsth.html

TS:   const PI: number = 3.14159;
来源：http://hz.ybcxt.top/gtksztugcz.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtbkdoqwhf.html

Go:   const PI = 3.14159
来源：http://hz.hammf.cn/gtkwscphtv.html

Ruby: PI = 3.14159
来源：http://hz.xylfe.cn/gttptrooje.html

C#:   const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtqycwxlgm.html

[A04] 判断变量类型
来源：http://hz.svipenyu.cn/gticiljpnu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinyuanbaomall.cn/gtimtcgziq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.andypj.xyz/gtjjmqzver.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hysaishi.cn/gtgwjkhkmi.html

TS:   typeof x; x instanceof Date
来源：http://hz.mhx1999.top/gtvhdjigns.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yanxiufei.cn/gtggltfxaz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.kuanghao11.cn/gtfyesoojr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxuanxn.top/gtinqxdzip.html

C#:   x.GetType().Name; x is int
来源：http://hz.xziqi.cn/gtsegyavll.html

[A05] 整数除法与取模
来源：http://hz.yuanzhike.top/gtwwoyzxhq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xylfe.cn/gtpnzngwag.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.bjfxy.top/gtdzkzdbwu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pycfn.com/gtryxxdtdb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtyqagvyvg.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gtspbpiudf.html

Go:   7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtrwaygcfp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtqirddkep.html

C#:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtpjuylhmj.html

[A06] 字符串转数字
来源：http://hz.yueranfly.top/gtsaoapsih.html

Py:   int("42"); float("3.14")
来源：http://hz.yuanzhike.top/gtwuesrwrh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gaohongyu789.top/gttbdtuegr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xziqi.cn/gttdsoojkv.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gtedtydqao.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yj20258888.top/gtuocpvyuw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.vqdsnc.cn/gtsqrxqwlw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.vqdsnc.cn/gtnpsfkxsm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinyuanbaomall.cn/gtvbnxmrpu.html

[A07] 数字转字符串
来源：http://hz.ybcxt.top/gtnlpjsbhz.html

Py:   str(42)
来源：http://hz.hfpthk.cn/gtgzsynzwy.html

PHP:  (string) 42; strval(42)
来源：http://hz.hywenlv.cn/gtsiskyvxv.html

JS:   String(42); (42).toString()
来源：http://hz.iojbl.cn/gtsdkcmyoq.html

TS:   String(42)
来源：http://hz.daria6918.cn/gtsvcbjsty.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.chenjidiqi.icu/gtpmidyedf.html

Go:   strconv.Itoa(42)
来源：http://hz.zhixingplan.top/gtjrjabcta.html

Ruby: 42.to_s
来源：http://hz.gzhubu.top/gtzyqczjod.html

C#:   42.ToString()
来源：http://hz.hywenlv.cn/gtfsqyyoeo.html

[A08] 取整与四舍五入
来源：http://hz.zhixingplan.top/gttazfduki.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jiagoushi.top/gtfwltxnbq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.andypj.xyz/gttitqrfjv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yonumen.top/gtvtgmaahg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.quarkkingdee.top/gtxnljxkxf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.daxiang520.top/gtwxqqvxoc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.chenzaomai.com/gttuoysldv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.nanxinkj.top/gtielbnkzv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sysykeji.top/gtgobbryin.html

[A09] 绝对值与最大最小值
来源：http://hz.tianlin.xyz/gtxoobadyn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtbcitkfdr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gaohongyu789.top/gtmowouqda.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yj20258888.top/gtdydxfkru.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhongyouzk.top/gtxetxbdxq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinqigufen.top/gtcfcdxrvz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yongpay.top/gtmxituwvt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.9152youxi.cn/gtkxpgzyzz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ydjk.org.cn/gtyhhpwgjl.html

[A10] 生成随机数
来源：http://hz.nanxuanxn.top/gtanqqcqws.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ppjwa.cn/gttyzbntos.html

PHP:  random_int(1, 100);
来源：http://hz.vqdsnc.cn/gtvzbfyvzj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hnqzz.top/gteqtzjikr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.c1oappe.top/gtanptisnh.html

Java: new Random().nextInt(100) + 1
来源：http://hz.meibo888.top/gtpqbmtzec.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zycfv.cn/gtxsjodhbo.html

Ruby: rand(1..100)
来源：http://hz.fzhhl.top/gtqtisasjq.html

C#:   new Random().Next(1, 101)
来源：http://hz.shuidangran.top/gthjavowvj.html

[A11] 条件表达式（三元）
来源：http://hz.tianlin.xyz/gtveszhbqm.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhengqikj.top/gtpcrmbcak.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.wangdashe.top/gtbrziksqh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtmljvwszd.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gtuaquaugu.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtfmlkqsjp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.svipenyu.cn/gtkgurfnkr.html


<!-- 参考信息 -->