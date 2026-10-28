代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtqvnptgqc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shuidangran.top/gtjinshmtp.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtxhmsenzh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sxryk.cn/gtbdjcuwon.html

[U69] PHP：PDO 预处理
来源：http://hz.pengpengdd.cyou/gtznttlasr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtyvbpmbdq.html

[U70] PHP：PDO 事务
来源：http://hz.iojbl.cn/gtiexaxjlr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258.top/gtdusbikgr.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtnjxhskpu.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtgwednaxc.html

[U72] PHP：写错误日志
来源：http://hz.zhiwuduotai.top/gtnioibmer.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shangyingyoupin.top/gtoducocny.html

[U73] PHP：读取 ini 配置
来源：http://hz.wangdashe.top/gtvachutgq.html

parse_ini_file("config.ini", true)
来源：http://hz.yvedp.cn/gtqpihluli.html

[U74] PHP：读取环境变量
来源：http://hz.yuanzhike.top/gtdepodzqk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.pycfn.com/gtajsqpvzj.html

[U75] PHP：依赖注入
来源：http://hz.cashguo.top/gtyvyuqglr.html

composer require psr/container
来源：http://hz.jinyuanbaomall.cn/gtehgyaxab.html

[U76] PHP：简单路由
来源：http://hz.jinghuilouyu.cn/gtfjiagtxq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jyoumei.cn/gtjizlnsdr.html

[U77] PHP：模板渲染
来源：http://hz.9152youxi.cn/gtkutrjfxm.html

composer require twig/twig
来源：http://hz.52xcode.cn/gttfzkuref.html

[U78] PHP：单元测试
来源：http://hz.xinyue.icu/gtgkpwpixe.html

composer require --dev phpunit/phpunit
来源：http://hz.smart0.xyz/gtbamzkseu.html

[U79] PHP：静态分析
来源：http://hz.smart0.xyz/gtymqvmwuf.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtgyhznths.html

[U80] PHP：代码规范修复
来源：http://hz.yanxiufei.cn/gtlxdgunvr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sysykeji.top/gttagooswp.html

[U81] JS：初始化项目
来源：http://hz.wangdashe.top/gtqzpghmcu.html

npm init -y;  npm i express
来源：http://hz.ydzc1.top/gtzvnfggei.html

[U82] JS：package.json 脚本
来源：http://hz.sysykeji.top/gtudvwkyfl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.dianchejie.cn/gtwoishkpz.html

[U83] JS：ES Module 导入导出
来源：http://hz.xziqi.cn/gttbqbbhil.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.smart0.xyz/gtebequylz.html

[U84] JS：CommonJS 写法
来源：http://hz.chenzaomai.com/gtprszimsr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hammf.cn/gtelksxoqz.html

[U85] JS：可选链
来源：http://hz.aibaodan.cn/gtbocqnbvr.html

a?.b?.c
来源：http://hz.xingfuxueyuan.xyz/gtdajfaslk.html

[U86] JS：空值合并
来源：http://hz.zhiwuduotai.top/gtcufbmneb.html

a ?? b
来源：http://hz.iojbl.cn/gtnboemvvy.html

[U87] JS：解构默认值
来源：http://hz.yuanzhike.top/gtwsjkzfeu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daria6918.cn/gtpmmtkxyt.html

[U88] JS：对象展开合并
来源：http://hz.jyoumei.cn/gtnsfivbey.html

{ ...a, ...b }
来源：http://hz.ydzc1.top/gtrybhlwpl.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtllsdvtab.html

[...new Set(arr)]
来源：http://hz.yangfankeji.com/gtorzzjwii.html

[U90] JS：数字数组排序
来源：http://hz.yonumen.top/gtfflwimfg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtdzxytkhf.html

[U91] JS：对象键值遍历
来源：http://hz.zdqjudy.top/gtdboxrcez.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yj20258.top/gtdxghzukq.html

[U92] JS：深拷贝
来源：http://hz.yueranfly.top/gtrruxyuui.html

structuredClone(obj)
来源：http://hz.c1oappe.top/gtplgxbgqn.html

[U93] JS：模板字符串
来源：http://hz.jinqigfzy.top/gtufwgnoxs.html

`共 ${n} 条`
来源：http://hz.nanxinkj.top/gtjwgzynrk.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtxxcnkqlc.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gtwcfugpdx.html

[U95] JS：Promise 包装
来源：http://hz.yongpay.top/gthgwqghwd.html

new Promise((resolve, reject) => {})
来源：http://hz.jianghu66.top/gtpljeqwwe.html

[U96] JS：async/await 与异常
来源：http://hz.sysykeji.top/gtlujkyzth.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtbjiqkysq.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangtech.top/gtifgdtttw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtzxejfwcw.html

[U98] JS：fetch 带 JSON
来源：http://hz.guannengcc.top/gtofzqquno.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydjk.org.cn/gtznviebxp.html

[U99] JS：事件监听
来源：http://hz.mhx1999.top/gtwwteelnl.html

el.addEventListener("click", e => {})
来源：http://hz.chenlongwang.top/gtwiuvmecd.html

[U100] JS：DOM 查询
来源：http://hz.jlsjyb.cn/gtqemoncyr.html

document.querySelector(".item")
来源：http://hz.yuanzhike.top/gtngeqdmqr.html

[U101] JS：classList 操作
来源：http://hz.jinqigufen.top/gtzyrtgqnp.html

el.classList.toggle("active")
来源：http://hz.hongshengwenyu.top/gtlxicjwvc.html

[U102] JS：本地存储
来源：http://hz.chenlongwang.top/gtyngkioxp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yangfankeji.com/gtbbwirhlr.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtyobwqvud.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.0kj1m.cn/gtfugtfclu.html

[U104] JS：防抖
来源：http://hz.ydjk.org.cn/gtdsqnmrcb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtfsztbzcd.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gtyjlujacg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.smart0.xyz/gteboidpko.html

[U106] JS：日期格式化
来源：http://hz.kuanghao11.cn/gttvqavcse.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.kuanghao11.cn/gtsvosvvth.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtwuqrelhz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nwbrower.top/gtvieuriny.html

[U108] JS：随机整数
来源：http://hz.jinghuilouyu.cn/gtsbgxoori.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtkctkakam.html

[U109] JS：数组分组
来源：http://hz.sufxvd.cn/gtervrvqgb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gtpballejx.html

[U110] JS：数组分块
来源：http://hz.cqqwz.cn/gtkiakxvhm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.andypj.xyz/gtwrthhwvy.html

[U111] JS：对象转 Map
来源：http://hz.zhoulong.xyz/gtfckouzfc.html

new Map(Object.entries(obj))
来源：http://hz.ydzc1.top/gtebbvtkks.html

[U112] JS：字符串补位
来源：http://hz.jqgfzy.top/gtsbrnitus.html

"7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtaceymlqu.html

[U113] JS：正则替换全部
来源：http://hz.ydjk.org.cn/gtclqdkbjw.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtrypenpas.html

[U114] JS：JSON 深比较
来源：http://hz.zhoulong.xyz/gtatflsrle.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtrdyflvee.html

[U115] JS：生成 UUID
来源：http://hz.sweek.top/gtxxdbsdyw.html

crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtqtajzctl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gtounopojh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yangfankeji.com/gtvjqoqmum.html

[U117] JS：单元测试
来源：http://hz.sxryk.cn/gtiunzyjhq.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgufenzy.top/gtgeflyryd.html

[U118] JS：开发服务器
来源：http://hz.ivvv.top/gtdglsxfxt.html

npm i -D vite;  npx vite
来源：http://hz.chenlongwang.top/gtaksbpyld.html

[U119] JS：生产构建
来源：http://hz.andypj.xyz/gtirmepbhy.html

npx vite build
来源：http://hz.andypj.xyz/gtfdhkzsyv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ehwqpu.com/gtkqmrmsrl.html

import.meta.env.VITE_API_URL
来源：http://hz.yuanzhike.top/gtqtatfxzw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmgocjaac.html

统计汇总
来源：http://hz.jlsjyb.cn/gtlqqyfjwk.html

================================================================================
来源：http://hz.gotoacloud.top/gtkbjixzms.html

按语言统计（条）：
来源：http://hz.xingfuxueyuan.xyz/gtccfnljfy.html

Python ......... 252
来源：http://hz.zhaomingkeji.xyz/gthdkkyvdi.html

PHP ............ 252
来源：http://hz.tanke756.top/gtecocwxrq.html

JavaScript ..... 252
来源：http://hz.yongpay.top/gtufayurvp.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gtznwjozzv.html

Java ........... 212
来源：http://hz.snrcjt.cn/gtavdpbnlh.html

Go ............. 212
来源：http://hz.cashguo.top/gthktxxgph.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtvjmmbdnh.html

C# ............. 212
来源：http://hz.jlsjyb.cn/gtqrbcnnln.html

C .............. 30
来源：http://hz.zhaomingkeji.xyz/gtoydgglrh.html

C++ ............ 30
来源：http://hz.shanyushiyangkeji.top/gtzdudhhxa.html

SQL ............ 90
来源：http://hz.redwolf501.top/gtcxyhfepw.html

Bash ........... 80
来源：http://hz.ydzc1.top/gtluqvbmhs.html

Kotlin ......... 15
来源：http://hz.yvedp.cn/gtovnwoheo.html

Swift .......... 15
来源：http://hz.hammf.cn/gtiqacxazy.html

Lua ............ 10
来源：http://hz.jianghu66.top/gtzoqjgjkh.html

Perl ........... 10
来源：http://hz.fengsongda.top/gthbzpimac.html

Scala .......... 10
来源：http://hz.iojbl.cn/gtgsxbpuuk.html

------------------------------------
来源：http://hz.nanxinkj.top/gtjminzbwk.html

合计 ........... 2106 条
来源：http://hz.cashguo.top/gttjrhjprn.html

按章节统计：
来源：http://hz.gzhubu.top/gtjgcovyzf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtawxfszxh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtwcotodpc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtvfakhuuu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pycfn.com/gtvlydgbcm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.svipenyu.cn/gtvymtywas.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtqvowlpsd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtummxcesh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtqqpglvji.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gthddojlpl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.bjfxy.top/gthqvewnhd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtyijoylll.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtouyzhdin.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtpndwsvea.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtelluctum.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shzxlz.cn/gtvpvfkizf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtxbwfrgzw.html

Q SQL 专题                              90
来源：http://hz.andypj.xyz/gtzegkpcsw.html

R Bash 专题                             80
来源：http://hz.gogol.net.cn/gtuggcaniq.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtaboqknpo.html

T 其他语言补充                          60
来源：http://hz.zhoulong.xyz/gtvxgdykmi.html

U 高频实用片段                         120
来源：http://hz.jinqigufen.top/gtnysomlxi.html

------------------------------------
来源：http://hz.gotoacloud.top/gtknviyaby.html

合计                                  2106 条
来源：http://hz.jianghu66.top/gtshrbenhz.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtflsxjbvv.html

使用提醒
来源：http://hz.bjfxy.top/gttrswagon.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtnoldyscs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.aibaodan.cn/gtyoexzdpl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.havefunace.top/gtzifviyla.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xylfe.cn/gtyummzqtu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydzc1.top/gtkzbwcekw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.andypj.xyz/gtbeazbbkc.html

—— 文件结束 ——
来源：http://hz.tanke756.top/gtohwirdhi.html

================================================================================
来源：http://hz.yj202588.top/gtscwyjgin.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhoulong.xyz/gtvzxdntnb.html

Common Programming Examples Cheat Book
来源：http://hz.yuanzhike.top/gtezrfqmns.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmbveytik.html

【收录内容】
来源：http://hz.xziqi.cn/gtattuejlo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ydjk.org.cn/gtbapifxxi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nwbrower.top/gtwkelagkx.html

SQL · Bash · C · C++
来源：http://hz.sysykeji.top/gtyfhoaqre.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cucudq.cn/gtniqvovvr.html

【使用说明】
来源：http://hz.gzhubu.top/gtneivurkg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.fengsongda.top/gtxadcoabk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guannengcc.top/gtbeigmbdb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sysykeji.top/gtammhpqxl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yonumen.top/gtnijzbygd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yuxming.cn/gtiogveyzb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.pycfn.com/gteluhelpi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jlsjyb.cn/gtafbpvtyl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ydzc1.top/gtxtfrtumd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtvmkwitpq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.aibaodan.cn/gttdbflunh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xylfe.cn/gtlhmprtff.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.dianchejie.cn/gthwyttmzv.html

【文件统计】
来源：http://hz.c1oappe.top/gtjicppuqu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gotoacloud.top/gtmzdpmhbb.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtycistuym.html

目  录
来源：http://hz.yuanzhike.top/gtqfzqjbmq.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtwizaawuc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxinkj.top/gtfurljazb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtldsodbxl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtqhjvwiac.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gtsxwdbouw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gtfpibkiil.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.c1oappe.top/gtwdwedetj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtphlskevs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gtbppcnyza.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtuiovdghf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtfvjlljhy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtihkjqfob.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtcruaxdhw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gttjxxekcr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.andypj.xyz/gtfhhzutas.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtgbocoxac.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtfxkblmmo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gogol.net.cn/gtppzraitq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ybcxt.top/gtmzmvpkzp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtzhhqgihr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtavltdsyc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtnwregosw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlgertstu.html

A. 基础语法与类型
来源：http://hz.pycfn.com/gtgqjtgfxk.html

================================================================================
来源：http://hz.sysykeji.top/gthqsyerxf.html

[A01] Hello World
来源：http://hz.redwolf501.top/gtsdiukjww.html

Py:   print("Hello, World!")
来源：http://hz.yueranfly.top/gthfraziqp.html

PHP:  echo "Hello, World!";
来源：http://hz.aizwys.cn/gtdxtsavlc.html

JS:   console.log("Hello, World!");
来源：http://hz.cqqwz.cn/gtdvpvxrkr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.shangyingyoupin.top/gtrhrqwbxb.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj20258.top/gtorplrtii.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgfzy.top/gtupkshxty.html

Ruby: puts "Hello, World!"
来源：http://hz.sufxvd.cn/gtszudrywq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yueranfly.top/gtzbhfrcmn.html

[A02] 变量声明与赋值
来源：http://hz.fengsongda.top/gtjpiegwgl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ybcxt.top/gtvrrjuxfj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gzhubu.top/gtxlvvthjr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shzxlz.cn/gtaoxnbzue.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydjk.org.cn/gtxwsjmuho.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtyckvghhf.html

Go:   name := "Alex"; age := 20
来源：http://hz.vqdsnc.cn/gtcsjiarne.html

Ruby: name = "Alex"; age = 20
来源：http://hz.nanxuanxn.top/gtlqddufou.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sxryk.cn/gtscengqap.html

[A03] 常量定义
来源：http://hz.cdnleiting.top/gtdtndmcom.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yuanzhike.top/gtwuucdzok.html

PHP:  const PI = 3.14159;
来源：http://hz.smart0.xyz/gtaylypcqr.html

JS:   const PI = 3.14159;
来源：http://hz.tian-w.cn/gtjbnjrqqx.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtvertcxan.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtavfhuvxn.html

Go:   const PI = 3.14159
来源：http://hz.jinqigfzy.top/gtflcltshe.html

Ruby: PI = 3.14159
来源：http://hz.dashuyun.cn/gtjhkhtyqj.html

C#:   const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtqfojtucl.html

[A04] 判断变量类型
来源：http://hz.zhixingplan.top/gtxnpspfqp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aibaodan.cn/gtrdulszsk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hammf.cn/gtheyuhrfc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinyuanbaomall.cn/gthsigcbog.html

TS:   typeof x; x instanceof Date
来源：http://hz.yangfankeji.com/gtxudpxexi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.mhx1999.top/gtobrshviu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.daria6918.cn/gtahpygpss.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.guowangkeji.top/gtfouxgsfn.html

C#:   x.GetType().Name; x is int
来源：http://hz.snrcjt.cn/gtcmlcnecm.html

[A05] 整数除法与取模
来源：http://hz.jqgfzy.top/gtjhbwhyck.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yuxming.cn/gtsntugynw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.chenlongwang.top/gtjgzgpgdi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cucudq.cn/gtplrtcuay.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtxfedatsq.html

Java: 7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtiwkrnpho.html

Go:   7 / 2; 7 % 2
来源：http://hz.meibo888.top/gthtzrbrae.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.52xcode.cn/gtpkvmfdud.html

C#:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtgqcxerrt.html

[A06] 字符串转数字
来源：http://hz.hnqzz.top/gtilngojqq.html

Py:   int("42"); float("3.14")
来源：http://hz.hnqzz.top/gtgrqzupfd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.andypj.xyz/gtqiiobbrd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yj20258.top/gtmyzsptdn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.dashuyun.cn/gtbfycmlxk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.kuanghao11.cn/gteyqohhfv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jianghu66.top/gtrtnacdan.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.daria6918.cn/gtjdlsnxfw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cheryme.top/gtcnlofrqd.html

[A07] 数字转字符串
来源：http://hz.sufxvd.cn/gtrlzkmoqo.html

Py:   str(42)
来源：http://hz.daxiang520.top/gttzlgkpgr.html

PHP:  (string) 42; strval(42)
来源：http://hz.quarkkingdee.top/gtkzxbrjml.html

JS:   String(42); (42).toString()
来源：http://hz.cdnleiting.top/gtlgamjcjk.html

TS:   String(42)
来源：http://hz.ybcxt.top/gtwfookjgm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xuetiantiany.cn/gtykhqtrhx.html

Go:   strconv.Itoa(42)
来源：http://hz.ivvv.top/gtdezutksz.html

Ruby: 42.to_s
来源：http://hz.xziqi.cn/gtzyekiiae.html

C#:   42.ToString()
来源：http://hz.zhongyouzk.top/gtbnbzorza.html

[A08] 取整与四舍五入
来源：http://hz.zhiwuduotai.top/gtieszblmb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hfpthk.cn/gtrtdbkkqs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.meibo888.top/gtzobikgkl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.tian-w.cn/gtofyusklf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.daria6918.cn/gtqquusgsr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhiwuduotai.top/gttftglboz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yonumen.top/gtetkyvukv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.xziqi.cn/gtujbbrcax.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jiagoushi.top/gtvsriiqxx.html

[A09] 绝对值与最大最小值
来源：http://hz.ydzc1.top/gtmzaldsnt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.guowangkeji.top/gtsaewbdll.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yonumen.top/gtwbboamhk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yuxming.cn/gtklbcndvr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.havefunace.top/gtvedioohc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.guowangkeji.top/gtxglqsehq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yuxming.cn/gtepbhbakl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yongpay.top/gthlwrrbgi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.dianchejie.cn/gtbshykrky.html

[A10] 生成随机数
来源：http://hz.hfpthk.cn/gtdfjmdpdd.html

Py:   import random; random.randint(1, 100)
来源：http://hz.dashuyun.cn/gtjcnyhpvy.html

PHP:  random_int(1, 100);
来源：http://hz.aibaodan.cn/gtkxarxlos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ehwqpu.com/gtjuqfyaao.html


<!-- 参考信息 -->