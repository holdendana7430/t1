代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtdsisaaqg.html

parse_ini_file("config.ini", true)
来源：http://hz.tanke756.top/gtipmxujdp.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangtech.top/gtdavlftgy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yanxiufei.cn/gtxdgofyof.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gtpwiwryvb.html

composer require psr/container
来源：http://hz.zhengqikj.top/gtpvtmeozp.html

[U76] PHP：简单路由
来源：http://hz.nanxuanxn.top/gtzwstxmre.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.meibo888.top/gtefjkgvil.html

[U77] PHP：模板渲染
来源：http://hz.smart0.xyz/gtltwdclra.html

composer require twig/twig
来源：http://hz.yj20258888.top/gtwfzhhzqd.html

[U78] PHP：单元测试
来源：http://hz.ehwqpu.com/gttvslhpbo.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtaopmsjjd.html

[U79] PHP：静态分析
来源：http://hz.jiagoushi.top/gttmhdtdvu.html

composer require --dev phpstan/phpstan
来源：http://hz.jianghu66.top/gtalizxrxi.html

[U80] PHP：代码规范修复
来源：http://hz.kuanghao11.cn/gtiturdtyi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yonumen.top/gtgehfxhfz.html

[U81] JS：初始化项目
来源：http://hz.ydzc1.top/gtxioswpuz.html

npm init -y;  npm i express
来源：http://hz.zhijiandao.cn/gttkvcllvx.html

[U82] JS：package.json 脚本
来源：http://hz.jyoumei.cn/gtwcpuqxni.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.smart0.xyz/gtxvmtrcyc.html

[U83] JS：ES Module 导入导出
来源：http://hz.shuidangran.top/gtaaqohfju.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.snrcjt.cn/gtnobeqhso.html

[U84] JS：CommonJS 写法
来源：http://hz.haohaochexian.top/gthvamktpg.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xinyue.icu/gtkvscsvaz.html

[U85] JS：可选链
来源：http://hz.ivvv.top/gtovasxhqf.html

a?.b?.c
来源：http://hz.jinyuanbaomall.cn/gtoswciwor.html

[U86] JS：空值合并
来源：http://hz.redwolf501.top/gtuevptubl.html

a ?? b
来源：http://hz.cashguo.top/gtdxognria.html

[U87] JS：解构默认值
来源：http://hz.zhongyouzk.top/gttcnackls.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yongpay.top/gtwcevbudv.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtlvepvzht.html

{ ...a, ...b }
来源：http://hz.xinyue.icu/gtjoktyzyi.html

[U89] JS：数组去重
来源：http://hz.jiagoushi.top/gtycviuxrm.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtdpgphauc.html

[U90] JS：数字数组排序
来源：http://hz.shzxlz.cn/gtxpuxhtba.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtghwiqids.html

[U91] JS：对象键值遍历
来源：http://hz.dashuyun.cn/gtjyvbkcnf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtypppvqaz.html

[U92] JS：深拷贝
来源：http://hz.fengsongda.top/gtsbupeyfg.html

structuredClone(obj)
来源：http://hz.haohaochexian.top/gtychnzdwv.html

[U93] JS：模板字符串
来源：http://hz.pengpengdd.cyou/gtbomlocdf.html

`共 ${n} 条`
来源：http://hz.yueranfly.top/gtjpulyxbc.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gtzfleyzdp.html

const double = x => x * 2;
来源：http://hz.jlsjyb.cn/gtwoaxuzfh.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtkioovczw.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtlwzhqboo.html

[U96] JS：async/await 与异常
来源：http://hz.havefunace.top/gtsvxlikgr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtrchlkfix.html

[U97] JS：并发请求
来源：http://hz.cdnleiting.top/gtputyicxt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtjwxlofps.html

[U98] JS：fetch 带 JSON
来源：http://hz.andypj.xyz/gtyilgmvrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ppjwa.cn/gtbfufcxin.html

[U99] JS：事件监听
来源：http://hz.pycfn.com/gtrelufciy.html

el.addEventListener("click", e => {})
来源：http://hz.cheryme.top/gtpzsbwlum.html

[U100] JS：DOM 查询
来源：http://hz.nanxinkj.top/gtqtgsamqu.html

document.querySelector(".item")
来源：http://hz.c1oappe.top/gtkrdllihb.html

[U101] JS：classList 操作
来源：http://hz.hfpthk.cn/gtdwraasxy.html

el.classList.toggle("active")
来源：http://hz.ppjwa.cn/gtbzeclgzk.html

[U102] JS：本地存储
来源：http://hz.tianlin.xyz/gtpaycmlbi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ivvv.top/gtadvlazkh.html

[U103] JS：定时器
来源：http://hz.aizwys.cn/gtaspokrtt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gaohongyu789.top/gtwibjgawb.html

[U104] JS：防抖
来源：http://hz.zhijiandao.cn/gtfevcxyjj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtwjqohczh.html

[U105] JS：节流
来源：http://hz.haohaochexian.top/gtnzbhpbsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydjk.org.cn/gtgmuykhkl.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtfjupkbwb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtnpveqztu.html

[U107] JS：数字千分位
来源：http://hz.shangyingyoupin.top/gtusppuslf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhongyouzk.top/gtzwchsoyh.html

[U108] JS：随机整数
来源：http://hz.cheryme.top/gtbomwjpga.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yanxiufei.cn/gtgtqybosz.html

[U109] JS：数组分组
来源：http://hz.zhongyouzk.top/gtqovumqbo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtumozvwpd.html

[U110] JS：数组分块
来源：http://hz.jyoumei.cn/gtkkqghvly.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.iojbl.cn/gtkfvrrhkg.html

[U111] JS：对象转 Map
来源：http://hz.yuanzhike.top/gtuhqguhdy.html

new Map(Object.entries(obj))
来源：http://hz.gzhubu.top/gtexdhvmlw.html

[U112] JS：字符串补位
来源：http://hz.andypj.xyz/gtosytuyco.html

"7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtekjtjbut.html

[U113] JS：正则替换全部
来源：http://hz.ppjwa.cn/gtrqtvvwyt.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gthjbdodhk.html

[U114] JS：JSON 深比较
来源：http://hz.gaohongyu789.top/gtxysrtnlg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtinnsdath.html

[U115] JS：生成 UUID
来源：http://hz.svipenyu.cn/gtcwreroeh.html

crypto.randomUUID()
来源：http://hz.bjfxy.top/gtjzlppaqx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gogol.net.cn/gtoixhxwli.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhongyouzk.top/gtxpomhavi.html

[U117] JS：单元测试
来源：http://hz.yangfankeji.com/gthyrdezkj.html

npm i -D vitest;  npx vitest
来源：http://hz.xziqi.cn/gtqptgeztz.html

[U118] JS：开发服务器
来源：http://hz.c1oappe.top/gtgfcwbdza.html

npm i -D vite;  npx vite
来源：http://hz.zhiwuduotai.top/gtmypqqplr.html

[U119] JS：生产构建
来源：http://hz.ydzc1.top/gtoagxabqo.html

npx vite build
来源：http://hz.xinyue.icu/gtbbmqudxd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sweek.top/gtrovzskyy.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gtnpaxnemu.html

================================================================================
来源：http://hz.chenlongwang.top/gtgnzfkmxi.html

统计汇总
来源：http://hz.sxryk.cn/gtnizfbejj.html

================================================================================
来源：http://hz.cucudq.cn/gtkoyndmxg.html

按语言统计（条）：
来源：http://hz.jinqigufen.top/gtrpkqofmr.html

Python ......... 252
来源：http://hz.xuetiantiany.cn/gtpeilpwiw.html

PHP ............ 252
来源：http://hz.zhengqikj.top/gtvkjrheqk.html

JavaScript ..... 252
来源：http://hz.gzhubu.top/gtiasfddgp.html

TypeScript ..... 212
来源：http://hz.vqdsnc.cn/gthwndcnri.html

Java ........... 212
来源：http://hz.sufxvd.cn/gtjhvdyeuz.html

Go ............. 212
来源：http://hz.316326.xyz/gtlbnnaegz.html

Ruby ........... 212
来源：http://hz.gzhubu.top/gtvkqsytcl.html

C# ............. 212
来源：http://hz.wangdashe.top/gtukkrtssv.html

C .............. 30
来源：http://hz.zhengqikj.top/gttaivjwuh.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gtkjuyznwr.html

SQL ............ 90
来源：http://hz.sweek.top/gtrzhfiuca.html

Bash ........... 80
来源：http://hz.jianghu66.top/gtcrmztcvi.html

Kotlin ......... 15
来源：http://hz.wangdashe.top/gttlqohznb.html

Swift .......... 15
来源：http://hz.yangfankeji.com/gtcnhrhfpc.html

Lua ............ 10
来源：http://hz.birdmap.top/gtmcshleqg.html

Perl ........... 10
来源：http://hz.cheryme.top/gtidzqremt.html

Scala .......... 10
来源：http://hz.chenzaomai.com/gtpxtxohrl.html

------------------------------------
来源：http://hz.ehwqpu.com/gtjbolsdpw.html

合计 ........... 2106 条
来源：http://hz.xingfuxueyuan.xyz/gtymhvfyov.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtuqioijfa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtshixtzvp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtbdnnvjpy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangdashe.top/gtyotvrwrj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gtbgsciyxq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.vqdsnc.cn/gtffniffap.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtzgmhtwvh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtwguufmpm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtzybirzzc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtbvygzjrd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gtdgvxnsqu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtkjhgaxkf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtqxbeitsi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtjuqvertp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pengpengdd.cyou/gtpvyvefzx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tian-w.cn/gtdftnipzt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gttfipwvtn.html

Q SQL 专题                              90
来源：http://hz.iojbl.cn/gtrosicbcy.html

R Bash 专题                             80
来源：http://hz.cdnleiting.top/gtwlysmdea.html

S C / C++ 专题                          60
来源：http://hz.dianchejie.cn/gtuijrtodn.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtjzpbwfgx.html

U 高频实用片段                         120
来源：http://hz.cucudq.cn/gtntqjmamc.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtuvhhnnwy.html

合计                                  2106 条
来源：http://hz.yonumen.top/gtyitkyhiy.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtxdthszkv.html

使用提醒
来源：http://hz.zhoulong.xyz/gthoyorvsq.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtzebpudas.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xinyue.icu/gtmjxxhfgc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.svipenyu.cn/gtdimhcjiw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.havefunace.top/gthnpztlgo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shanyushiyangtech.top/gtfpyzzajm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cheryme.top/gtfdccblgu.html

—— 文件结束 ——
来源：http://hz.chenjidiqi.icu/gtpoxzqxjv.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtowvzzole.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.c1oappe.top/gtzjchbrla.html

Common Programming Examples Cheat Book
来源：http://hz.gaohongyu789.top/gtvgcyfwxp.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtuytexqaw.html

【收录内容】
来源：http://hz.smart0.xyz/gteictfdfi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhiwuduotai.top/gtegfokmja.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.meibo888.top/gtkvlacezx.html

SQL · Bash · C · C++
来源：http://hz.redwolf501.top/gtfkgdhncx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jqgufenzy.top/gtrieicgmw.html

【使用说明】
来源：http://hz.jinqigufen.top/gtojyzzbsf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gtgletglop.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinghuilouyu.cn/gtsiycenmi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.daxiang520.top/gtyttuzijo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dashuyun.cn/gthnglniyw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zdqjudy.top/gtshlvztus.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtifvgpemb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj20258.top/gtltdtammc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tianlin.xyz/gtkwuockqh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yueranfly.top/gtiwddmfic.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhoulong.xyz/gtjuowvusl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.quarkkingdee.top/gtxvhhhadh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tianlin.xyz/gtjzerdezc.html

【文件统计】
来源：http://hz.kuanghao11.cn/gtercbdoaq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gtkkswzjsc.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gtuuyunxqy.html

目  录
来源：http://hz.svipenyu.cn/gtgwpwfxor.html

--------------------------------------------------------------------------------
来源：http://hz.zycfv.cn/gtpiclhmlz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtdtbdbgcq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtujpohwqe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.havefunace.top/gtuootjyhx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtvgxguaxy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxuanxn.top/gtnjmsxbyv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtjjtyryzz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuetiantiany.cn/gtaezoeinp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtsekgfdnq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtxtgnqoyq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtcredingk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtvqcryifr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtkwksectx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtvinhkxzc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.svipenyu.cn/gtftvctrpn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258.top/gthblupeyk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gteggmpuiu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fengsongda.top/gtqqpmoysc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nwbrower.top/gtinoggwtp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yonumen.top/gtdhiffayk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtwxrocxsz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gttjlmoyxs.html

================================================================================
来源：http://hz.zhijiandao.cn/gttrlsnxqm.html

A. 基础语法与类型
来源：http://hz.hongshengwenyu.top/gtdlwtehtl.html

================================================================================
来源：http://hz.zhixingplan.top/gtlpsbpwli.html

[A01] Hello World
来源：http://hz.shuidangran.top/gtretvuout.html

Py:   print("Hello, World!")
来源：http://hz.gaohongyu789.top/gtrzigcmjq.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxinkj.top/gtyzhzqszt.html

JS:   console.log("Hello, World!");
来源：http://hz.cucudq.cn/gtfedbbsyh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jqgufenzy.top/gtbjyzhpsf.html

Java: System.out.println("Hello, World!");
来源：http://hz.quarkkingdee.top/gtafllrpke.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.gogol.net.cn/gtqnbcxqfg.html

Ruby: puts "Hello, World!"
来源：http://hz.redwolf501.top/gtcrnpxilf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydzc1.top/gtijcsmcxb.html

[A02] 变量声明与赋值
来源：http://hz.sufxvd.cn/gtsznmpnfk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhijiandao.cn/gtymjsogsg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.52xcode.cn/gtlvzkjzmc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangkeji.top/gtmtwbxkaf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.sweek.top/gtdziwlfbp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.smart0.xyz/gtvlvpyfmd.html

Go:   name := "Alex"; age := 20
来源：http://hz.52xcode.cn/gtdfmcbiba.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gtsvurhohy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtfsjukrvz.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtxkoxiogj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuanzhike.top/gtprqibfze.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxinkj.top/gtgillvgbw.html

JS:   const PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtdbnxbqep.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtrfvljlhm.html

Java: static final double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtvecsrzqw.html

Go:   const PI = 3.14159
来源：http://hz.redwolf501.top/gtdwtwkqht.html

Ruby: PI = 3.14159
来源：http://hz.zhaomingkeji.xyz/gtwedexrfc.html

C#:   const double PI = 3.14159;
来源：http://hz.sysykeji.top/gtbidxfiil.html

[A04] 判断变量类型
来源：http://hz.birdmap.top/gtblcxupuq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yj202588.top/gtjubgvauz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hywenlv.cn/gtbpzrfzuu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.havefunace.top/gtctlptljb.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtiogwtgph.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinghuilouyu.cn/gtelwnowxf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cdnleiting.top/gtbkwnzxrc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.0kj1m.cn/gtccwxcwat.html

C#:   x.GetType().Name; x is int
来源：http://hz.gogol.net.cn/gtttkrgmdh.html

[A05] 整数除法与取模
来源：http://hz.shanyushiyangtech.top/gtqoxfrlkp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ybcxt.top/gtuqfikrhv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtdwygiwxh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtihlhtefk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtwzlmxnmv.html

Java: 7 / 2; 7 % 2
来源：http://hz.xuetiantiany.cn/gttdrdtaty.html

Go:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtpaaoxaof.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ehwqpu.com/gttfolksiq.html

C#:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtppzfcuxa.html

[A06] 字符串转数字
来源：http://hz.guannengcc.top/gtrfvndtow.html

Py:   int("42"); float("3.14")
来源：http://hz.kuanghao11.cn/gthwnbzduj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhoulong.xyz/gtktwcglda.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.gaohongyu789.top/gtsopojxgt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtxlrxkozr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xinyue.icu/gtpkscwcxs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtcuthsely.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hnxiangtu.top/gtjhitmtfb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zhixingplan.top/gtkslyrdyd.html

[A07] 数字转字符串
来源：http://hz.zhixingplan.top/gtqqwiqwjh.html

Py:   str(42)
来源：http://hz.316326.xyz/gtxoefjcdu.html

PHP:  (string) 42; strval(42)
来源：http://hz.gzhubu.top/gtzfswynjf.html

JS:   String(42); (42).toString()
来源：http://hz.jqgfzy.top/gtvtuauhsx.html

TS:   String(42)
来源：http://hz.birdmap.top/gtnklmmzuj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xingfuxueyuan.xyz/gtwpmpdsfy.html

Go:   strconv.Itoa(42)
来源：http://hz.jqgfzy.top/gtozocxcee.html

Ruby: 42.to_s
来源：http://hz.hammf.cn/gtpqrooozy.html

C#:   42.ToString()
来源：http://hz.jinghuilouyu.cn/gtdhnyvhzn.html

[A08] 取整与四舍五入
来源：http://hz.52xcode.cn/gtujamusvd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.daxiang520.top/gttkdstlja.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.quarkkingdee.top/gthtxhzafx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gaohongyu789.top/gtbhxcsudx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhixingplan.top/gtqxezzayl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zdqjudy.top/gtmiypumdv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yuanzhike.top/gtrosmzldy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.guowangkeji.top/gtsgjoziwu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.svipenyu.cn/gtvcigtycp.html

[A09] 绝对值与最大最小值
来源：http://hz.nanxuanxn.top/gtqvmqrsla.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ydzc1.top/gtoxcarcho.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.redwolf501.top/gtargnijxj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.svipenyu.cn/gtfkfxxqoz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yj202588.top/gtinuhcqww.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhoulong.xyz/gtspwitrhd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhengqikj.top/gtjowgnwkl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.vqdsnc.cn/gttwztbswo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hfpthk.cn/gtzmskkjcp.html

[A10] 生成随机数
来源：http://hz.hongshengwenyu.top/gtcqjizigw.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xuanzx.com/gtooddidyv.html

PHP:  random_int(1, 100);
来源：http://hz.cdnleiting.top/gtobfequnx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.fengsongda.top/gtozdgnmzj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cqqwz.cn/gtbsbewime.html

Java: new Random().nextInt(100) + 1
来源：http://hz.vqdsnc.cn/gtthksddiw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.shanyushiyangtech.top/gtzqtayrdc.html

Ruby: rand(1..100)
来源：http://hz.zhengqikj.top/gtscjtvzwf.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj202588.top/gtstwdvhij.html

[A11] 条件表达式（三元）
来源：http://hz.xinyue.icu/gtmaxhbiyn.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhaomingkeji.xyz/gtxovzhzzs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtxwjotmlt.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtxoxdccos.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangkeji.top/gtkvknwkyc.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.gotoacloud.top/gtnuayyeiy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.cheryme.top/gtaiosewxx.html


<!-- 参考信息 -->