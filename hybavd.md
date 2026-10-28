代发 wailian999

[U63] PHP：文件读写
来源：http://hz.tanke756.top/gtrwpokdzw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gtoqwnayzy.html

[U64] PHP：目录遍历
来源：http://hz.jqgufenzy.top/gthcispoht.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shangyingyoupin.top/gtuothvpbk.html

[U65] PHP：会话
来源：http://hz.jianghu66.top/gtjpshpjmo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jiagoushi.top/gtcmxkqtsm.html

[U66] PHP：设置 Cookie
来源：http://hz.feifeiyinyue.top/gtcexhyppy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xinyue.icu/gtgrmreoeb.html

[U67] PHP：处理文件上传
来源：http://hz.dianchejie.cn/gtdnimyseq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jianghu66.top/gtgueqdgum.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigfzy.top/gtrxapewud.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtmmqtgtsu.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtkkmxxhzr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sxryk.cn/gtyryizelm.html

[U70] PHP：PDO 事务
来源：http://hz.andypj.xyz/gtsgtpcxjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fzhhl.top/gttvnggcio.html

[U71] PHP：抛出异常
来源：http://hz.yuanzhike.top/gtwwfyfiby.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuanzx.com/gtviqjmhil.html

[U72] PHP：写错误日志
来源：http://hz.xinyue.icu/gtjehidpda.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jianghu66.top/gtyulbdsow.html

[U73] PHP：读取 ini 配置
来源：http://hz.nanxuanxn.top/gtfkvihkhj.html

parse_ini_file("config.ini", true)
来源：http://hz.xziqi.cn/gtwepxzojc.html

[U74] PHP：读取环境变量
来源：http://hz.hammf.cn/gtkvdsonau.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xylfe.cn/gtcxhdpqml.html

[U75] PHP：依赖注入
来源：http://hz.guowangkeji.top/gtargzzzke.html

composer require psr/container
来源：http://hz.gaohongyu789.top/gtunqbccgo.html

[U76] PHP：简单路由
来源：http://hz.ywan-chungtsiang.top/gtshtlotxj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.vqdsnc.cn/gthjhkyscb.html

[U77] PHP：模板渲染
来源：http://hz.pengpengdd.cyou/gtrpscvocd.html

composer require twig/twig
来源：http://hz.tianlin.xyz/gtkrspphud.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtqeazajdx.html

composer require --dev phpunit/phpunit
来源：http://hz.yanxiufei.cn/gtsflkkimi.html

[U79] PHP：静态分析
来源：http://hz.jinqigufen.top/gtfkyxqehr.html

composer require --dev phpstan/phpstan
来源：http://hz.ydzc1.top/gtqtnbprvk.html

[U80] PHP：代码规范修复
来源：http://hz.tianlin.xyz/gtoziuydgn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.bjfxy.top/gthlkapadk.html

[U81] JS：初始化项目
来源：http://hz.guowangkeji.top/gtsglvvcwu.html

npm init -y;  npm i express
来源：http://hz.chenlongwang.top/gtjkukzzao.html

[U82] JS：package.json 脚本
来源：http://hz.mhx1999.top/gtlvgnvlng.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj20258.top/gtwoqupxjt.html

[U83] JS：ES Module 导入导出
来源：http://hz.andypj.xyz/gtjurzvozf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangtech.top/gthhlnpgaa.html

[U84] JS：CommonJS 写法
来源：http://hz.tanke756.top/gtwpqqeico.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hfpthk.cn/gtwyyxfxzj.html

[U85] JS：可选链
来源：http://hz.hywenlv.cn/gtgfaaxxhj.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtatpeufdz.html

[U86] JS：空值合并
来源：http://hz.tianlin.xyz/gtzfhlwnop.html

a ?? b
来源：http://hz.hywenlv.cn/gtfpvpzdpl.html

[U87] JS：解构默认值
来源：http://hz.cheryme.top/gtccvdcvwu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gtxjeqlgok.html

[U88] JS：对象展开合并
来源：http://hz.hnxiangtu.top/gtzshmtuvu.html

{ ...a, ...b }
来源：http://hz.guowangkeji.top/gttiewfrbq.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gtltfxkaym.html

[...new Set(arr)]
来源：http://hz.daxiang520.top/gtnfqgycev.html

[U90] JS：数字数组排序
来源：http://hz.dashuyun.cn/gtluipaohe.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gteroxjjsj.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258.top/gtqqwykkcv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zycfv.cn/gtsqevimac.html

[U92] JS：深拷贝
来源：http://hz.sufxvd.cn/gtshcmwiyj.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtleosvgza.html

[U93] JS：模板字符串
来源：http://hz.sweek.top/gtsjgmetmp.html

`共 ${n} 条`
来源：http://hz.xinyue.icu/gtgqpwirna.html

[U94] JS：箭头函数
来源：http://hz.hnxiangtu.top/gtypmlpbjn.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtcavxovtq.html

[U95] JS：Promise 包装
来源：http://hz.jinyuanbaomall.cn/gtehjfhuuw.html

new Promise((resolve, reject) => {})
来源：http://hz.aizwys.cn/gtoiatoxqt.html

[U96] JS：async/await 与异常
来源：http://hz.gaohongyu789.top/gtkyxygcvj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtwgokornm.html

[U97] JS：并发请求
来源：http://hz.zhongyouzk.top/gtuhelmrff.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gttyilglor.html

[U98] JS：fetch 带 JSON
来源：http://hz.nanxuanxn.top/gtbjslwzlt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtippyzqvb.html

[U99] JS：事件监听
来源：http://hz.aizwys.cn/gttbbjievv.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gtkufebqii.html

[U100] JS：DOM 查询
来源：http://hz.hammf.cn/gtmidwnowd.html

document.querySelector(".item")
来源：http://hz.sysykeji.top/gtxgayiwoy.html

[U101] JS：classList 操作
来源：http://hz.pengpengdd.cyou/gtbrdoifbc.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtnlsygyzc.html

[U102] JS：本地存储
来源：http://hz.yuanzhike.top/gtylumvwpf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigfzy.top/gtryayeukc.html

[U103] JS：定时器
来源：http://hz.hongshengwenyu.top/gtpyntdlzt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gaohongyu789.top/gtkwfkwcna.html

[U104] JS：防抖
来源：http://hz.ehwqpu.com/gtjikzbdgx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtzburtluw.html

[U105] JS：节流
来源：http://hz.zhiwuduotai.top/gtucpnwkvh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nanxinkj.top/gtfounlpww.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtkdkcbaef.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.bjfxy.top/gtadfqaaat.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtxrvjrhqu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yangfankeji.com/gtvmglbnbx.html

[U108] JS：随机整数
来源：http://hz.ywan-chungtsiang.top/gtujzsqkye.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.c1oappe.top/gtypvstnie.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gthwiesgdt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtixdsboix.html

[U110] JS：数组分块
来源：http://hz.jiagoushi.top/gtyecdlecb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tian-w.cn/gtdeftbsyl.html

[U111] JS：对象转 Map
来源：http://hz.sweek.top/gtemsmexrw.html

new Map(Object.entries(obj))
来源：http://hz.xuetiantiany.cn/gthbkxhkux.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtrchobqbs.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gteisdmkai.html

[U113] JS：正则替换全部
来源：http://hz.xinyue.icu/gtclngdesv.html

s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtbvcnjpgj.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gtdklwlbcm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtmfhhbrxf.html

[U115] JS：生成 UUID
来源：http://hz.shzxlz.cn/gtqqrmgadd.html

crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtzokvylmm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtlaaixgcn.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gogol.net.cn/gtdkiascyf.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gtxccmuhhd.html

npm i -D vitest;  npx vitest
来源：http://hz.c1oappe.top/gtqnzauibo.html

[U118] JS：开发服务器
来源：http://hz.ydzc1.top/gtpryacccm.html

npm i -D vite;  npx vite
来源：http://hz.xingfuxueyuan.xyz/gtlvihfguj.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtybsllofx.html

npx vite build
来源：http://hz.zhongyouzk.top/gtyumrmagj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jianghu66.top/gthmqqtqjt.html

import.meta.env.VITE_API_URL
来源：http://hz.xylfe.cn/gtqfyjzqrz.html

================================================================================
来源：http://hz.gaohongyu789.top/gthjfyxrkt.html

统计汇总
来源：http://hz.316326.xyz/gtzmigfnko.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtipidschi.html

按语言统计（条）：
来源：http://hz.shuidangran.top/gtxptglkyu.html

Python ......... 252
来源：http://hz.wangdashe.top/gtkdkdufta.html

PHP ............ 252
来源：http://hz.zhixingplan.top/gtawwubsrc.html

JavaScript ..... 252
来源：http://hz.guowangkeji.top/gtcmcxvrke.html

TypeScript ..... 212
来源：http://hz.gotoacloud.top/gtnmsxnizd.html

Java ........... 212
来源：http://hz.haohaochexian.top/gtwrczqonx.html

Go ............. 212
来源：http://hz.bjfxy.top/gtyjktvlna.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtvpjxbndz.html

C# ............. 212
来源：http://hz.gaohongyu789.top/gtdoylupyp.html

C .............. 30
来源：http://hz.jinqigufen.top/gtffvxogup.html

C++ ............ 30
来源：http://hz.aizwys.cn/gttnwbgjqe.html

SQL ............ 90
来源：http://hz.9152youxi.cn/gtnldimvoj.html

Bash ........... 80
来源：http://hz.yueranfly.top/gtiaommqgo.html

Kotlin ......... 15
来源：http://hz.ybcxt.top/gttdmssroc.html

Swift .......... 15
来源：http://hz.xingfuxueyuan.xyz/gttngiiktk.html

Lua ............ 10
来源：http://hz.hysaishi.cn/gttvyjztgo.html

Perl ........... 10
来源：http://hz.iojbl.cn/gtfqlhotuy.html

Scala .......... 10
来源：http://hz.xziqi.cn/gtpskzzide.html

------------------------------------
来源：http://hz.jinghuilouyu.cn/gtyioxemmy.html

合计 ........... 2106 条
来源：http://hz.zdqjudy.top/gtflqmjehm.html

按章节统计：
来源：http://hz.jinyuanbaomall.cn/gtcevmgyll.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtdwwchwza.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gteqsbwyay.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtnvgnufov.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtcbmotkxy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hongshengwenyu.top/gtyekthegf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gtbdipbzdn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtjvtocbzs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xuanzx.com/gtzqbypkai.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtcpkrqcoo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtbgudoyov.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtzkiyxnrg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtdprqkfqk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtrxigvmfv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtosszgoln.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.haohaochexian.top/gtctsomueh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtruggnggb.html

Q SQL 专题                              90
来源：http://hz.hnxiangtu.top/gtkuhtotxl.html

R Bash 专题                             80
来源：http://hz.gzhubu.top/gtdonhtxze.html

S C / C++ 专题                          60
来源：http://hz.c1oappe.top/gtlfjopjfd.html

T 其他语言补充                          60
来源：http://hz.zhiwuduotai.top/gthozmhhbr.html

U 高频实用片段                         120
来源：http://hz.316326.xyz/gttcoogtrs.html

------------------------------------
来源：http://hz.316326.xyz/gtwyohflhk.html

合计                                  2106 条
来源：http://hz.daxiang520.top/gtkdtnozgv.html

--------------------------------------------------------------------------------
来源：http://hz.yongpay.top/gtngyovxbm.html

使用提醒
来源：http://hz.jqgfzy.top/gtligeoval.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtpafexxin.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuxming.cn/gtvzcclnwj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hammf.cn/gtusfpcghm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dianchejie.cn/gttyiahery.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.iojbl.cn/gtwqhlseeq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.snrcjt.cn/gtbqloidsl.html

—— 文件结束 ——
来源：http://hz.gaohongyu789.top/gtinmhmxab.html

================================================================================
来源：http://hz.svipenyu.cn/gtsbrrlvcx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtedanwzir.html

Common Programming Examples Cheat Book
来源：http://hz.zhiwuduotai.top/gtyiswelpu.html

================================================================================
来源：http://hz.fzhhl.top/gtytubmhok.html

【收录内容】
来源：http://hz.hysaishi.cn/gtdphafvri.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.redwolf501.top/gtdcxlvzqy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.9152youxi.cn/gtubfychkf.html

SQL · Bash · C · C++
来源：http://hz.iojbl.cn/gtizrhvjwh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinyuanbaomall.cn/gtpkmzgtij.html

【使用说明】
来源：http://hz.xuanzx.com/gtwhpbwdmd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shzxlz.cn/gtkcrpwitt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.wangdashe.top/gtufpqoded.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtuzxuufmz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tianlin.xyz/gtlkqpbpfc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.svipenyu.cn/gttprnrars.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tanke756.top/gtqtbxlxtk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangdashe.top/gtisarlick.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gthsrwzbwl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtsshacvsc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tanke756.top/gtqcyawbty.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgfzy.top/gtoobwkadp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xziqi.cn/gtwdsipajo.html

【文件统计】
来源：http://hz.yonumen.top/gtyejmpajv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ivvv.top/gthmfxdamw.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtpoplkowl.html

目  录
来源：http://hz.ybcxt.top/gtigarpdlb.html

--------------------------------------------------------------------------------
来源：http://hz.ywan-chungtsiang.top/gtouzzvfwo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.andypj.xyz/gtvhcsitso.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtlnnpjqjy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtyofnqjrk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.pengpengdd.cyou/gtpbnzvpre.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxinkj.top/gtekfswpey.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtujqxschm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtmyngrcaw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nwbrower.top/gtzayixbxi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtrcmzband.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtzkdkpxfp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtoxqlyczf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtibwhdqno.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtypcjmqnm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhijiandao.cn/gtyavpjqmy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.vqdsnc.cn/gtvsgqdmub.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtrzolsyca.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shangyingyoupin.top/gtefaikldj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.dashuyun.cn/gtdzolemqr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xinyue.icu/gtyfarbecn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtnehtkpgq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtasrvfruo.html

================================================================================
来源：http://hz.pycfn.com/gtgjvaswur.html

A. 基础语法与类型
来源：http://hz.gaohongyu789.top/gtgougbiyi.html

================================================================================
来源：http://hz.316326.xyz/gtwesouhzh.html

[A01] Hello World
来源：http://hz.ydjk.org.cn/gtdcskmafb.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtehkkgrrj.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtaewzfmji.html

JS:   console.log("Hello, World!");
来源：http://hz.gaohongyu789.top/gtpmcrpwqj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zycfv.cn/gtjxbzndux.html

Java: System.out.println("Hello, World!");
来源：http://hz.hnxiangtu.top/gtsdmcjdzb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cdnleiting.top/gtwhcewbhf.html

Ruby: puts "Hello, World!"
来源：http://hz.shanyushiyangkeji.top/gtzqgcfzyg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xingfuxueyuan.xyz/gtcwhmhfxv.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gthoprozro.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sxryk.cn/gtqwsxriql.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.snrcjt.cn/gtsupkpuzf.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yanxiufei.cn/gtecibwdwe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ywan-chungtsiang.top/gtxumemfea.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.meibo888.top/gtrospuwtp.html

Go:   name := "Alex"; age := 20
来源：http://hz.ydjk.org.cn/gtbjmudxgu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.birdmap.top/gtxbauuuoa.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.quarkkingdee.top/gtdqogwtqj.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gtihofekyy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj20258888.top/gtlfxgrprr.html

PHP:  const PI = 3.14159;
来源：http://hz.mhx1999.top/gtslnpzvpf.html

JS:   const PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtwxchtjby.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtowfxfoyx.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigufen.top/gthhaphehg.html

Go:   const PI = 3.14159
来源：http://hz.9152youxi.cn/gtodfqpcku.html

Ruby: PI = 3.14159
来源：http://hz.redwolf501.top/gtldyqwyul.html

C#:   const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtnrydkdej.html

[A04] 判断变量类型
来源：http://hz.birdmap.top/gtqucpfvvm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnqzz.top/gtbcjbsrjx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.c1oappe.top/gtfuunafgo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zdqjudy.top/gtlvgopdad.html

TS:   typeof x; x instanceof Date
来源：http://hz.nanxinkj.top/gtvtkooeri.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ydjk.org.cn/gttkgdujsa.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hammf.cn/gtjngaovrq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yj202588.top/gtxhxpirwg.html

C#:   x.GetType().Name; x is int
来源：http://hz.yuanzhike.top/gtpkslqtjr.html

[A05] 整数除法与取模
来源：http://hz.zycfv.cn/gttvmbukqz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.havefunace.top/gtqtjkqeic.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zycfv.cn/gtrcxmtwfd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtqvnjvqes.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hammf.cn/gtysssrohd.html

Java: 7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtyebnzkun.html

Go:   7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtpaciasuu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtnnjkvziu.html

C#:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtziomjkdw.html

[A06] 字符串转数字
来源：http://hz.jianghu66.top/gtmvcwxkce.html

Py:   int("42"); float("3.14")
来源：http://hz.cashguo.top/gtjfvmeftt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.chenzaomai.com/gtpnbydwje.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinqigufen.top/gtlpjdmnlj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.shanyushiyangkeji.top/gtfwfllofs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yj20258.top/gtnpxdjwsa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.guowangkeji.top/gtbdowlnka.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sysykeji.top/gtofxfmiai.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.havefunace.top/gtqieoemcl.html

[A07] 数字转字符串
来源：http://hz.c1oappe.top/gtuwloqeqg.html

Py:   str(42)
来源：http://hz.shuidangran.top/gtraxvmxyr.html

PHP:  (string) 42; strval(42)
来源：http://hz.svipenyu.cn/gtuulzugaw.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangtech.top/gtrmiiomcn.html

TS:   String(42)
来源：http://hz.birdmap.top/gtehuvjxyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.0kj1m.cn/gthibqxata.html

Go:   strconv.Itoa(42)
来源：http://hz.yj20258.top/gtuhacdnix.html

Ruby: 42.to_s
来源：http://hz.havefunace.top/gtnvkswytp.html

C#:   42.ToString()
来源：http://hz.haohaochexian.top/gthsrodsqi.html

[A08] 取整与四舍五入
来源：http://hz.xylfe.cn/gtwsdykcbt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xylfe.cn/gtuozzpcsm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yvedp.cn/gtuwybssjl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cqqwz.cn/gtqkqzedum.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangkeji.top/gtdxnvihcv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yuxming.cn/gtxlxulevi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.feifeiyinyue.top/gtmeihgaro.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yongpay.top/gtreecphys.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ydjk.org.cn/gthkhuqium.html

[A09] 绝对值与最大最小值
来源：http://hz.yuxming.cn/gtakodpkqw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jiagoushi.top/gtzgzdtyrz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.smart0.xyz/gtrdjsdymp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hongshengwenyu.top/gtjqlhhoyw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nwbrower.top/gtmlnmhnkf.html


<!-- 参考信息 -->