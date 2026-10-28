代发 wailian999

[U67] PHP：处理文件上传
来源：http://hz.0kj1m.cn/gtuyggwvlc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtczaalznr.html

[U68] PHP：PDO 连接
来源：http://hz.vqdsnc.cn/gtkvlrhrza.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtrivkveeh.html

[U69] PHP：PDO 预处理
来源：http://hz.jinqigufen.top/gtrslztcgv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtkalaodhv.html

[U70] PHP：PDO 事务
来源：http://hz.guowangkeji.top/gtpofgdbmi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtxjfaekvp.html

[U71] PHP：抛出异常
来源：http://hz.yongpay.top/gtfvzvpicf.html

throw new RuntimeException("失败", 500);
来源：http://hz.tian-w.cn/gtcgsbbdyg.html

[U72] PHP：写错误日志
来源：http://hz.ivvv.top/gtedicsmji.html

error_log("失败: " . $e->getMessage());
来源：http://hz.bjfxy.top/gtelzxkpvl.html

[U73] PHP：读取 ini 配置
来源：http://hz.guowangkeji.top/gtiwsrfinr.html

parse_ini_file("config.ini", true)
来源：http://hz.cdnleiting.top/gtippzywab.html

[U74] PHP：读取环境变量
来源：http://hz.quarkkingdee.top/gtomgwjltu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.snrcjt.cn/gttbilgkmk.html

[U75] PHP：依赖注入
来源：http://hz.hnqzz.top/gtlyufyrnz.html

composer require psr/container
来源：http://hz.shzxlz.cn/gttzbwzgwf.html

[U76] PHP：简单路由
来源：http://hz.hywenlv.cn/gtjhfaunot.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.316326.xyz/gtdayirxyp.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gtmkvxzvna.html

composer require twig/twig
来源：http://hz.sweek.top/gtpzfpogqj.html

[U78] PHP：单元测试
来源：http://hz.zdqjudy.top/gtxexfpmtr.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gtolxjcrsb.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gtfyaxxzdz.html

composer require --dev phpstan/phpstan
来源：http://hz.redwolf501.top/gtdtwfjpal.html

[U80] PHP：代码规范修复
来源：http://hz.cqqwz.cn/gtjpvxvhwr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.birdmap.top/gtcxvllgad.html

[U81] JS：初始化项目
来源：http://hz.cashguo.top/gtfpthfzkf.html

npm init -y;  npm i express
来源：http://hz.smart0.xyz/gtasjwjsle.html

[U82] JS：package.json 脚本
来源：http://hz.nwbrower.top/gthfgxkqtx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhixingplan.top/gtgglvllwe.html

[U83] JS：ES Module 导入导出
来源：http://hz.zycfv.cn/gtswbwbhpr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.feifeiyinyue.top/gtcpcbbaes.html

[U84] JS：CommonJS 写法
来源：http://hz.feifeiyinyue.top/gtltudbyuu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gaohongyu789.top/gtvaewwjdg.html

[U85] JS：可选链
来源：http://hz.ybcxt.top/gtcsvrqeny.html

a?.b?.c
来源：http://hz.zhijiandao.cn/gtnsajtjfb.html

[U86] JS：空值合并
来源：http://hz.hammf.cn/gtfxsbceqs.html

a ?? b
来源：http://hz.jlsjyb.cn/gtreexnszw.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtcwhhuqno.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangdashe.top/gthmtlshgd.html

[U88] JS：对象展开合并
来源：http://hz.hysaishi.cn/gtzitvcgzt.html

{ ...a, ...b }
来源：http://hz.aizwys.cn/gtaoizfxjx.html

[U89] JS：数组去重
来源：http://hz.zhijiandao.cn/gtqqcnkyvr.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtoslnvrht.html

[U90] JS：数字数组排序
来源：http://hz.fengsongda.top/gtmczlkypo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtyomuwyga.html

[U91] JS：对象键值遍历
来源：http://hz.zhoulong.xyz/gtowdunixp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yonumen.top/gthsvkjsot.html

[U92] JS：深拷贝
来源：http://hz.yvedp.cn/gtouiesgre.html

structuredClone(obj)
来源：http://hz.daxiang520.top/gttoihnapb.html

[U93] JS：模板字符串
来源：http://hz.gaohongyu789.top/gtvpsnuixh.html

`共 ${n} 条`
来源：http://hz.hongshengwenyu.top/gtizxvkacu.html

[U94] JS：箭头函数
来源：http://hz.redwolf501.top/gtntuplcfs.html

const double = x => x * 2;
来源：http://hz.dashuyun.cn/gtdklybvzz.html

[U95] JS：Promise 包装
来源：http://hz.hongshengwenyu.top/gtugjizntd.html

new Promise((resolve, reject) => {})
来源：http://hz.ydjk.org.cn/gtkgflzoaq.html

[U96] JS：async/await 与异常
来源：http://hz.tanke756.top/gtnjelomxs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtklsgxkie.html

[U97] JS：并发请求
来源：http://hz.shzxlz.cn/gtajjiikgn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtqppwfhso.html

[U98] JS：fetch 带 JSON
来源：http://hz.sweek.top/gtqmrkkzcc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.wangdashe.top/gtvcvtpopk.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtwvdpotsb.html

el.addEventListener("click", e => {})
来源：http://hz.xingfuxueyuan.xyz/gtjzeugxms.html

[U100] JS：DOM 查询
来源：http://hz.andypj.xyz/gtloscchtu.html

document.querySelector(".item")
来源：http://hz.jianghu66.top/gtgandoizq.html

[U101] JS：classList 操作
来源：http://hz.hnqzz.top/gtlxvmiyjd.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtaosjxiut.html

[U102] JS：本地存储
来源：http://hz.cucudq.cn/gteadmmgkl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nwbrower.top/gtclgjnuxi.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtxshkrqyc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhengqikj.top/gtuwuswufx.html

[U104] JS：防抖
来源：http://hz.havefunace.top/gtefufdqht.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtzqsdowco.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gtzcowmuap.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigufen.top/gtyxpmdrgu.html

[U106] JS：日期格式化
来源：http://hz.dashuyun.cn/gtssvnvgtt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangdashe.top/gtrnqbbimg.html

[U107] JS：数字千分位
来源：http://hz.hysaishi.cn/gtbppjvvni.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.0kj1m.cn/gtzsjyxlvk.html

[U108] JS：随机整数
来源：http://hz.mhx1999.top/gtvbtvbzmp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtsbmudvfd.html

[U109] JS：数组分组
来源：http://hz.tianlin.xyz/gtuxsvlrlp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gttzncipxx.html

[U110] JS：数组分块
来源：http://hz.xuanzx.com/gtsggbhjaw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nwbrower.top/gthegdkqpp.html

[U111] JS：对象转 Map
来源：http://hz.yangfankeji.com/gtrbddxnvw.html

new Map(Object.entries(obj))
来源：http://hz.zhengqikj.top/gthvgtszjo.html

[U112] JS：字符串补位
来源：http://hz.guowangkeji.top/gtzryxmzei.html

"7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtylkiekhy.html

[U113] JS：正则替换全部
来源：http://hz.hnqzz.top/gtcisgytns.html

s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtewwatxas.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtbuwocvzl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtkyqovskf.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtqgpnkiol.html

crypto.randomUUID()
来源：http://hz.nwbrower.top/gtfjflpokw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sxryk.cn/gtadgzovhr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtgailcxbx.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtnzbeydyt.html

npm i -D vitest;  npx vitest
来源：http://hz.sysykeji.top/gthnormbqi.html

[U118] JS：开发服务器
来源：http://hz.jlsjyb.cn/gttoaagjoo.html

npm i -D vite;  npx vite
来源：http://hz.xinyue.icu/gtuyucuwrl.html

[U119] JS：生产构建
来源：http://hz.zhaomingkeji.xyz/gtkedugokk.html

npx vite build
来源：http://hz.jyoumei.cn/gtxowufvqt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.fengsongda.top/gtacyumwnp.html

import.meta.env.VITE_API_URL
来源：http://hz.yuanzhike.top/gtopokfzsq.html

================================================================================
来源：http://hz.mhx1999.top/gtgzkbqfhu.html

统计汇总
来源：http://hz.jinqigufen.top/gtjrfupjre.html

================================================================================
来源：http://hz.shuidangran.top/gtwclnpruz.html

按语言统计（条）：
来源：http://hz.cdnleiting.top/gtnkleduqk.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtlfymwhdt.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtnwcvhvgt.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtcbihqrvv.html

TypeScript ..... 212
来源：http://hz.ivvv.top/gtpbtxxllw.html

Java ........... 212
来源：http://hz.redwolf501.top/gtpvhbwaxa.html

Go ............. 212
来源：http://hz.jiagoushi.top/gtsqscrdhd.html

Ruby ........... 212
来源：http://hz.snrcjt.cn/gtgkklmttz.html

C# ............. 212
来源：http://hz.shuidangran.top/gtpgifqdqm.html

C .............. 30
来源：http://hz.svipenyu.cn/gtroiggkef.html

C++ ............ 30
来源：http://hz.zhoulong.xyz/gtxwqrjlva.html

SQL ............ 90
来源：http://hz.hywenlv.cn/gtaqbhlxql.html

Bash ........... 80
来源：http://hz.ydjk.org.cn/gtvsxdosbb.html

Kotlin ......... 15
来源：http://hz.yongpay.top/gtrwwwhyqm.html

Swift .......... 15
来源：http://hz.pengpengdd.cyou/gthvkckjtn.html

Lua ............ 10
来源：http://hz.xylfe.cn/gteiacvjmc.html

Perl ........... 10
来源：http://hz.yueranfly.top/gtnqlhkwqz.html

Scala .......... 10
来源：http://hz.bjfxy.top/gthntljumz.html

------------------------------------
来源：http://hz.meibo888.top/gthqimntpw.html

合计 ........... 2106 条
来源：http://hz.sysykeji.top/gtrkvzdmei.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtqohfwbhd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtizpqxess.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtjcwysqhz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtjgdmpzns.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtuwkxrxai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pycfn.com/gtftipvumb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtazzebada.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtapythldy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.kuanghao11.cn/gtuutodsxm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtqtxtmjqn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shzxlz.cn/gtfjnwssro.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtytvtfdub.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtnvrflqbc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtsuzqamqc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gthelmcsqa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.0kj1m.cn/gtwdfbrbxr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtqcwfknms.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtizuuzowo.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gtpwewjyfk.html

S C / C++ 专题                          60
来源：http://hz.aizwys.cn/gtynzhxjmy.html

T 其他语言补充                          60
来源：http://hz.gaohongyu789.top/gtzofjkxiy.html

U 高频实用片段                         120
来源：http://hz.tanke756.top/gtakjlpttd.html

------------------------------------
来源：http://hz.yvedp.cn/gthiwabaab.html

合计                                  2106 条
来源：http://hz.haohaochexian.top/gtxbylyeso.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtscripcvv.html

使用提醒
来源：http://hz.vqdsnc.cn/gtbkkyybdb.html

--------------------------------------------------------------------------------
来源：http://hz.yangfankeji.com/gtkabfcuij.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ppjwa.cn/gtahioclxr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cheryme.top/gtrwkcnoyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yueranfly.top/gtdgkugjnu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cucudq.cn/gtxgydpfzg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ehwqpu.com/gtlwbhgrvs.html

—— 文件结束 ——
来源：http://hz.snrcjt.cn/gtqusllsyd.html

================================================================================
来源：http://hz.hammf.cn/gttfkisxot.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xuetiantiany.cn/gtpxrnbncc.html

Common Programming Examples Cheat Book
来源：http://hz.shanyushiyangkeji.top/gtbwqkmlvk.html

================================================================================
来源：http://hz.fzhhl.top/gthaosywuz.html

【收录内容】
来源：http://hz.cashguo.top/gtqtstadix.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zdqjudy.top/gtldzzwhla.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.feifeiyinyue.top/gtgknixsds.html

SQL · Bash · C · C++
来源：http://hz.smart0.xyz/gtucqxsfsu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenlongwang.top/gtfsiqtenv.html

【使用说明】
来源：http://hz.shuidangran.top/gtutubnxcy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.fzhhl.top/gtgggsgjpm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtxvrkkcmg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gtljsxodlt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aibaodan.cn/gtfbjxivry.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinyuanbaomall.cn/gtygxbwlcu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tian-w.cn/gtcegtmlvk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.iojbl.cn/gtzisnlyod.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.havefunace.top/gtxqdtubeb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hysaishi.cn/gtanozzepr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gzhubu.top/gtnasnuggn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.9152youxi.cn/gtziwncpal.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.quarkkingdee.top/gtsbqjwlze.html

【文件统计】
来源：http://hz.chenzaomai.com/gtgcuhkcok.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.hongshengwenyu.top/gtbxkhgqyj.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gttbmlldbc.html

目  录
来源：http://hz.aizwys.cn/gtbnktrjnv.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtabqhqkde.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gttieoydag.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtcyylkztj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtbyszkojb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gtqysvklcj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pycfn.com/gthfurlraj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hammf.cn/gtphdtwaly.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtrukdbvoz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtxlepxwma.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtioeluxwu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhongyouzk.top/gtxnerlaec.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtgvdpatbq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtfitwybqk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtqlbiuyln.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hywenlv.cn/gtwqjhaumy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hnxiangtu.top/gtyucuyttb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtepxjumec.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cheryme.top/gtuaivsiyo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jinyuanbaomall.cn/gtnvjiessq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxuanxn.top/gtqixuhitw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gthnkxcfxh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtjjbpyysq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnwjxfixf.html

A. 基础语法与类型
来源：http://hz.iojbl.cn/gtduepmgft.html

================================================================================
来源：http://hz.tianlin.xyz/gtqapdpprk.html

[A01] Hello World
来源：http://hz.cucudq.cn/gtcuyzyujc.html

Py:   print("Hello, World!")
来源：http://hz.bjfxy.top/gtfvqhqyxy.html

PHP:  echo "Hello, World!";
来源：http://hz.hysaishi.cn/gtyqkcnvtu.html

JS:   console.log("Hello, World!");
来源：http://hz.meibo888.top/gtuekaxcgq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenzaomai.com/gtqwgojuqb.html

Java: System.out.println("Hello, World!");
来源：http://hz.ydjk.org.cn/gtmxpwszbg.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.redwolf501.top/gtkivxionb.html

Ruby: puts "Hello, World!"
来源：http://hz.c1oappe.top/gtcpkvhjcx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.haohaochexian.top/gtzmyrqevh.html

[A02] 变量声明与赋值
来源：http://hz.hongshengwenyu.top/gthkukinod.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtqvnvgqwk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zdqjudy.top/gtollfdaca.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.dashuyun.cn/gtzlmfihlw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cashguo.top/gtqwrgnkcy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daria6918.cn/gtpfhlahvi.html

Go:   name := "Alex"; age := 20
来源：http://hz.vqdsnc.cn/gtybfgqpdk.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cqqwz.cn/gtwlrzlqty.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yongpay.top/gthdwrvwhb.html

[A03] 常量定义
来源：http://hz.zhengqikj.top/gtmqlttjio.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.nanxinkj.top/gtwnrttdyo.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtabapjqla.html

JS:   const PI = 3.14159;
来源：http://hz.wangdashe.top/gtqoambbgq.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigufen.top/gtlodzjvub.html

Java: static final double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtzufdknqx.html

Go:   const PI = 3.14159
来源：http://hz.hywenlv.cn/gtjjcffnkg.html

Ruby: PI = 3.14159
来源：http://hz.pengpengdd.cyou/gtmponhgox.html

C#:   const double PI = 3.14159;
来源：http://hz.yonumen.top/gtblxazqgu.html

[A04] 判断变量类型
来源：http://hz.pengpengdd.cyou/gtysphjbqg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.bjfxy.top/gtvbrnggld.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ybcxt.top/gtfrmgrrrm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.haohaochexian.top/gtggkbkgsm.html

TS:   typeof x; x instanceof Date
来源：http://hz.cqqwz.cn/gtvhaurqnr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.9152youxi.cn/gthlrorvgh.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xuetiantiany.cn/gtlkxvfkhn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gtuzdklwuk.html

C#:   x.GetType().Name; x is int
来源：http://hz.xylfe.cn/gtlppzugmo.html

[A05] 整数除法与取模
来源：http://hz.xuanzx.com/gtqkgmoahx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zhijiandao.cn/gtgblyexfd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jyoumei.cn/gtjosapegm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jiagoushi.top/gtzvmwmrkd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtjmufskss.html

Java: 7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gtgsxxwjbt.html

Go:   7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtoxfybxfl.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.snrcjt.cn/gtnjulkwjl.html

C#:   7 / 2; 7 % 2
来源：http://hz.tianlin.xyz/gttalglypr.html

[A06] 字符串转数字
来源：http://hz.zhixingplan.top/gtuziicbzg.html

Py:   int("42"); float("3.14")
来源：http://hz.ehwqpu.com/gteptxjchv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.quarkkingdee.top/gtcdkowxdl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sufxvd.cn/gtymhxqjss.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.chenlongwang.top/gtwtgcgbqo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hfpthk.cn/gtiyzlagpp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.quarkkingdee.top/gtyldeiwkq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ehwqpu.com/gtubqapzit.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shuidangran.top/gtkositgnr.html

[A07] 数字转字符串
来源：http://hz.xinyue.icu/gtpottgarr.html

Py:   str(42)
来源：http://hz.hnqzz.top/gtxvfzsfvw.html

PHP:  (string) 42; strval(42)
来源：http://hz.yanxiufei.cn/gtdiviggpv.html

JS:   String(42); (42).toString()
来源：http://hz.yj202588.top/gtjuztnunq.html

TS:   String(42)
来源：http://hz.mhx1999.top/gtoytznrcy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.52xcode.cn/gtfzoafqsg.html

Go:   strconv.Itoa(42)
来源：http://hz.hnxiangtu.top/gtvhxebuad.html

Ruby: 42.to_s
来源：http://hz.kuanghao11.cn/gtnhryjpla.html

C#:   42.ToString()
来源：http://hz.cashguo.top/gtflejiqit.html

[A08] 取整与四舍五入
来源：http://hz.shuidangran.top/gtoogikopb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ppjwa.cn/gtlkmqxgid.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yuxming.cn/gtmyvmtomz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.fengsongda.top/gtnmaagutl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.0kj1m.cn/gtlgfpjkar.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hfpthk.cn/gtodjbfasd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jqgufenzy.top/gtclbaajot.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zhoulong.xyz/gtxkiiuxtj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.quarkkingdee.top/gtiyipnask.html

[A09] 绝对值与最大最小值
来源：http://hz.ydjk.org.cn/gthxtdqtfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.vqdsnc.cn/gtnqkamwyo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgufenzy.top/gtroyjyvdt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.chenzaomai.com/gtkhsyqcqx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.feifeiyinyue.top/gtcnofjwwf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jqgfzy.top/gtwmlmhsoh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.guowangkeji.top/gtukwnbndp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hnqzz.top/gtdkrlbyct.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zdqjudy.top/gtpqdtjhxa.html

[A10] 生成随机数
来源：http://hz.ydjk.org.cn/gtarwazzpv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ehwqpu.com/gtnhenkcjc.html

PHP:  random_int(1, 100);
来源：http://hz.xinyue.icu/gtkxomltdj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gtcimucvvq.html


<!-- 参考信息 -->