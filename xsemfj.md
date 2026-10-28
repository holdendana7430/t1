代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.shzxlz.cn/gtvfwjvsqo.html

"值: {$a}"
来源：http://hz.yueranfly.top/gtnyefyjzu.html

[U58] PHP：数组三件套
来源：http://hz.meibo888.top/gtjsgnsidm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ydzc1.top/gtwashuipv.html

[U59] PHP：自定义排序
来源：http://hz.shangyingyoupin.top/gtigsyxqhf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtkbtncnlj.html

[U60] PHP：JSON 编解码
来源：http://hz.52xcode.cn/gtnaqwtehy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nwbrower.top/gtlwptjehk.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtvvjjmeex.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtbjfvrypx.html

[U62] PHP：日期对象
来源：http://hz.xingfuxueyuan.xyz/gtbnbfzvhg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zdqjudy.top/gthfyvcxax.html

[U63] PHP：文件读写
来源：http://hz.redwolf501.top/gtomsqomca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhongyouzk.top/gtmknzqitc.html

[U64] PHP：目录遍历
来源：http://hz.pengpengdd.cyou/gtabfouopz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.fzhhl.top/gtztrzfgzx.html

[U65] PHP：会话
来源：http://hz.havefunace.top/gtvjbytpir.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.quarkkingdee.top/gtjgxccxja.html

[U66] PHP：设置 Cookie
来源：http://hz.chenzaomai.com/gtyanfxzyi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.mhx1999.top/gtqtlcekou.html

[U67] PHP：处理文件上传
来源：http://hz.shuidangran.top/gtszkrmebo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.andypj.xyz/gtzywywkiy.html

[U68] PHP：PDO 连接
来源：http://hz.mhx1999.top/gtqrfiaoye.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yueranfly.top/gtytjecflx.html

[U69] PHP：PDO 预处理
来源：http://hz.hywenlv.cn/gtnfpvwutm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yanxiufei.cn/gtmwtfvpgo.html

[U70] PHP：PDO 事务
来源：http://hz.yvedp.cn/gtieqhlmec.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtjdgtjeuc.html

[U71] PHP：抛出异常
来源：http://hz.zhongyouzk.top/gtdliznorm.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigfzy.top/gtgeamtwcl.html

[U72] PHP：写错误日志
来源：http://hz.aizwys.cn/gtdzqfjoxi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.andypj.xyz/gtmhbcvagc.html

[U73] PHP：读取 ini 配置
来源：http://hz.yvedp.cn/gtxhpqaahk.html

parse_ini_file("config.ini", true)
来源：http://hz.pengpengdd.cyou/gtuwszzccq.html

[U74] PHP：读取环境变量
来源：http://hz.yonumen.top/gtwxfuznag.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtdmqjfkum.html

[U75] PHP：依赖注入
来源：http://hz.xziqi.cn/gtlhhpfhni.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtygyrtsmq.html

[U76] PHP：简单路由
来源：http://hz.yvedp.cn/gturgfferi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.haohaochexian.top/gtekowetcc.html

[U77] PHP：模板渲染
来源：http://hz.yongpay.top/gtsirbihaq.html

composer require twig/twig
来源：http://hz.pycfn.com/gtgmimngxh.html

[U78] PHP：单元测试
来源：http://hz.havefunace.top/gtwmrwdkll.html

composer require --dev phpunit/phpunit
来源：http://hz.daxiang520.top/gtbrkuedum.html

[U79] PHP：静态分析
来源：http://hz.ivvv.top/gtbzdxrizf.html

composer require --dev phpstan/phpstan
来源：http://hz.gzhubu.top/gtedzpekmb.html

[U80] PHP：代码规范修复
来源：http://hz.hnxiangtu.top/gtuiozlnjt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.dashuyun.cn/gtiivvvarr.html

[U81] JS：初始化项目
来源：http://hz.pycfn.com/gtluxzrkel.html

npm init -y;  npm i express
来源：http://hz.dashuyun.cn/gtwmbwpbes.html

[U82] JS：package.json 脚本
来源：http://hz.316326.xyz/gteuypzngz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xuetiantiany.cn/gtsphyrhpm.html

[U83] JS：ES Module 导入导出
来源：http://hz.guannengcc.top/gtklskmewa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.havefunace.top/gtwtklvccd.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtmjaqdwbs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinghuilouyu.cn/gtwvtnccqh.html

[U85] JS：可选链
来源：http://hz.sufxvd.cn/gtskjbuqdu.html

a?.b?.c
来源：http://hz.zhongyouzk.top/gtkznoqvti.html

[U86] JS：空值合并
来源：http://hz.52xcode.cn/gtippeuult.html

a ?? b
来源：http://hz.gogol.net.cn/gtvyidlpvs.html

[U87] JS：解构默认值
来源：http://hz.dashuyun.cn/gtlebgohhv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daxiang520.top/gtvqwgoqhj.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtqzvkdfdu.html

{ ...a, ...b }
来源：http://hz.dianchejie.cn/gttnpgrvov.html

[U89] JS：数组去重
来源：http://hz.hnxiangtu.top/gtorydckat.html

[...new Set(arr)]
来源：http://hz.chenlongwang.top/gtqjdpccsw.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangkeji.top/gteobjqkec.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtkoxyxvwh.html

[U91] JS：对象键值遍历
来源：http://hz.jianghu66.top/gtctyxtxwe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangtech.top/gtaltzfglx.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtlxeijaht.html

structuredClone(obj)
来源：http://hz.gzhubu.top/gtutkaarwy.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtvexvjmym.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gtpfawaqtg.html

[U94] JS：箭头函数
来源：http://hz.sweek.top/gtnhgydupy.html

const double = x => x * 2;
来源：http://hz.sxryk.cn/gtvvxxafhj.html

[U95] JS：Promise 包装
来源：http://hz.jqgufenzy.top/gthhmasykd.html

new Promise((resolve, reject) => {})
来源：http://hz.sysykeji.top/gtvobkuxqq.html

[U96] JS：async/await 与异常
来源：http://hz.hywenlv.cn/gteldmtxwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtdepyvqgi.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtuignmcwy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtwdpqrrwi.html

[U98] JS：fetch 带 JSON
来源：http://hz.tian-w.cn/gtgkpmaflc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.9152youxi.cn/gtjdczpsjz.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtrvptdbaq.html

el.addEventListener("click", e => {})
来源：http://hz.jlsjyb.cn/gtvbedaocz.html

[U100] JS：DOM 查询
来源：http://hz.chenlongwang.top/gtcqcmflon.html

document.querySelector(".item")
来源：http://hz.tanke756.top/gtrammnjfq.html

[U101] JS：classList 操作
来源：http://hz.chenlongwang.top/gteovgxbtj.html

el.classList.toggle("active")
来源：http://hz.jyoumei.cn/gtgwqpjcom.html

[U102] JS：本地存储
来源：http://hz.xziqi.cn/gtvvphmvpc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gogol.net.cn/gtnxqsoxht.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtmjnpakxl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jyoumei.cn/gtyxyiusdx.html

[U104] JS：防抖
来源：http://hz.zycfv.cn/gtkcdzlkqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gttosytzbh.html

[U105] JS：节流
来源：http://hz.xziqi.cn/gtayjyoruj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gtnjnbqmqj.html

[U106] JS：日期格式化
来源：http://hz.0kj1m.cn/gtiikxuryx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tianlin.xyz/gthrptvrel.html

[U107] JS：数字千分位
来源：http://hz.yuanzhike.top/gtifgpifcm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangshuangyany.cn/gtvrmyltih.html

[U108] JS：随机整数
来源：http://hz.jinqigufen.top/gtzwpnakpi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shuidangran.top/gtekavsdmi.html

[U109] JS：数组分组
来源：http://hz.hnxiangtu.top/gtcvqvdwts.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtuqqgcgdn.html

[U110] JS：数组分块
来源：http://hz.cashguo.top/gtribwjxwx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.vqdsnc.cn/gthogvmttj.html

[U111] JS：对象转 Map
来源：http://hz.jyoumei.cn/gteffgmnam.html

new Map(Object.entries(obj))
来源：http://hz.snrcjt.cn/gtsmebmvwf.html

[U112] JS：字符串补位
来源：http://hz.smart0.xyz/gtbfffhiha.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtkrqoogil.html

[U113] JS：正则替换全部
来源：http://hz.fengsongda.top/gtmxukeepz.html

s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtspeajcda.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtgurzrsef.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtkvmezefn.html

[U115] JS：生成 UUID
来源：http://hz.aibaodan.cn/gtachuzxuf.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtdjbabqpu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sufxvd.cn/gtlhrqweey.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shzxlz.cn/gtpvealisc.html

[U117] JS：单元测试
来源：http://hz.gaohongyu789.top/gtdcczrbgz.html

npm i -D vitest;  npx vitest
来源：http://hz.hysaishi.cn/gtbgfzpaja.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gtgblyevfd.html

npm i -D vite;  npx vite
来源：http://hz.hysaishi.cn/gtaqvirpue.html

[U119] JS：生产构建
来源：http://hz.yvedp.cn/gtsneweegk.html

npx vite build
来源：http://hz.zhaomingkeji.xyz/gtnjndgxag.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shuidangran.top/gtduhfcvhg.html

import.meta.env.VITE_API_URL
来源：http://hz.yvedp.cn/gtvnhcknss.html

================================================================================
来源：http://hz.c1oappe.top/gtlomauuzj.html

统计汇总
来源：http://hz.yanxiufei.cn/gtsbvdzwjh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtklkauqnq.html

按语言统计（条）：
来源：http://hz.tian-w.cn/gtkafqpsbp.html

Python ......... 252
来源：http://hz.shanyushiyangtech.top/gtuuxchfmw.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtficzagld.html

JavaScript ..... 252
来源：http://hz.gotoacloud.top/gtzcccbdky.html

TypeScript ..... 212
来源：http://hz.hywenlv.cn/gtbevfcjrl.html

Java ........... 212
来源：http://hz.xuetiantiany.cn/gtfbkyiybn.html

Go ............. 212
来源：http://hz.shanyushiyangtech.top/gtbnigldsz.html

Ruby ........... 212
来源：http://hz.meibo888.top/gturahehms.html

C# ............. 212
来源：http://hz.jinqigufen.top/gtjwqmaiyz.html

C .............. 30
来源：http://hz.jinyuanbaomall.cn/gtvuysphee.html

C++ ............ 30
来源：http://hz.gaohongyu789.top/gtrlbdzrum.html

SQL ............ 90
来源：http://hz.ydjk.org.cn/gtgiqzzvpc.html

Bash ........... 80
来源：http://hz.c1oappe.top/gtmzorbjpc.html

Kotlin ......... 15
来源：http://hz.wangdashe.top/gtknlwacbq.html

Swift .......... 15
来源：http://hz.haohaochexian.top/gtpkzbcevd.html

Lua ............ 10
来源：http://hz.smart0.xyz/gttriljycw.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtelidocbv.html

Scala .......... 10
来源：http://hz.daria6918.cn/gtjnbrsgkj.html

------------------------------------
来源：http://hz.0kj1m.cn/gtitvxullu.html

合计 ........... 2106 条
来源：http://hz.kuanghao11.cn/gtgezarjzm.html

按章节统计：
来源：http://hz.redwolf501.top/gtceifxcgs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhongyouzk.top/gtrpccigkw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtqgfnpqan.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gthkeqzccm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtulpamrnp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtbiynmivu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hnqzz.top/gtmhotvxxz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtgurrrvju.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtzwtyetrs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtzhtxppmb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hnxiangtu.top/gtiuhsjpqg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtqdmqwwzu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtbagollsq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtqycxtbmf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangkeji.top/gthtzatmbt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtapmceiyc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtzbkmsqiz.html

Q SQL 专题                              90
来源：http://hz.cdnleiting.top/gtmjcfnmcj.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtrmuihffr.html

S C / C++ 专题                          60
来源：http://hz.xuetiantiany.cn/gtvnfdtihx.html

T 其他语言补充                          60
来源：http://hz.jqgufenzy.top/gtyxtxuayl.html

U 高频实用片段                         120
来源：http://hz.tian-w.cn/gtdrmblsmt.html

------------------------------------
来源：http://hz.0kj1m.cn/gtrzrnabez.html

合计                                  2106 条
来源：http://hz.yuxming.cn/gtugnxlnjs.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtxtvltzmu.html

使用提醒
来源：http://hz.ehwqpu.com/gtkvcckriq.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtthoqigdc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sxryk.cn/gtccuidbst.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gtftwsmxks.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.xuetiantiany.cn/gttgjsnuao.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtnwovcrpz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xuetiantiany.cn/gtaqtsxrlr.html

—— 文件结束 ——
来源：http://hz.gogol.net.cn/gtodavnliq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzyagvelh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.dianchejie.cn/gtiaizanos.html

Common Programming Examples Cheat Book
来源：http://hz.jianghu66.top/gtmwflcjzz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjiieyjhu.html

【收录内容】
来源：http://hz.svipenyu.cn/gtfguogcgm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.fengsongda.top/gtffngjkvm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.dashuyun.cn/gtxaxjdwld.html

SQL · Bash · C · C++
来源：http://hz.redwolf501.top/gtcjkykkuw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhongyouzk.top/gtwktcujce.html

【使用说明】
来源：http://hz.cheryme.top/gtisnscoxr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zycfv.cn/gtbevjvcjk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.c1oappe.top/gtkrqjwort.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gttalhbmvo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cqqwz.cn/gtqgzocmif.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtzljjqhls.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.fzhhl.top/gtxmfsrvsg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ppjwa.cn/gtvgymydak.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jlsjyb.cn/gtnvzvzvui.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.birdmap.top/gtztnrblxw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhoulong.xyz/gthreonupo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.kuanghao11.cn/gtruuqpgjc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jiagoushi.top/gtlhdujmcx.html

【文件统计】
来源：http://hz.daxiang520.top/gtwpaqfnvx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jiagoushi.top/gthmqymaov.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtrmzqlqzx.html

目  录
来源：http://hz.redwolf501.top/gtksatqjsa.html

--------------------------------------------------------------------------------
来源：http://hz.wangshuangyany.cn/gtpiicyida.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtbaczteip.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gteksjkfqz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtjsigpyjc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtxojocuab.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtsvfbbguh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtgdvwhcsz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtiwtkhtwy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gaohongyu789.top/gtigniorxk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtjlsrvpfo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gthxdjljpt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtwmirkwwc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gthurzxuvn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtskrebygu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.aizwys.cn/gtnspaifsl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cdnleiting.top/gtueflstkt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtzaunxgfn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hfpthk.cn/gttdhystoj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.iojbl.cn/gtkwweshrf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hnxiangtu.top/gtvgwpkjqv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtqvfhwbyp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtgeylpanv.html

================================================================================
来源：http://hz.aizwys.cn/gtekjtenhh.html

A. 基础语法与类型
来源：http://hz.yvedp.cn/gtviuuhnbs.html

================================================================================
来源：http://hz.chenlongwang.top/gtfoezeymg.html

[A01] Hello World
来源：http://hz.guannengcc.top/gtlfmhczyz.html

Py:   print("Hello, World!")
来源：http://hz.zhijiandao.cn/gtfpkoezdi.html

PHP:  echo "Hello, World!";
来源：http://hz.sufxvd.cn/gtgslqqecw.html

JS:   console.log("Hello, World!");
来源：http://hz.fengsongda.top/gtskgqgnoj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hongshengwenyu.top/gttuywwlvs.html

Java: System.out.println("Hello, World!");
来源：http://hz.quarkkingdee.top/gtqflivymr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtjjtywrrm.html

Ruby: puts "Hello, World!"
来源：http://hz.jinqigfzy.top/gtcgdqmlmc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuxming.cn/gtjfyilivn.html

[A02] 变量声明与赋值
来源：http://hz.dianchejie.cn/gtqjrnilqw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zycfv.cn/gtupnquisb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.daxiang520.top/gtxyernknb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jianghu66.top/gtrcmhdhnt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yanxiufei.cn/gtjuqpyxyq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhixingplan.top/gtfvblydxv.html

Go:   name := "Alex"; age := 20
来源：http://hz.haohaochexian.top/gtcjwuhzja.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgfzy.top/gtrasiqucv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.daria6918.cn/gtrmouvxym.html

[A03] 常量定义
来源：http://hz.haohaochexian.top/gtfgiihcnu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenzaomai.com/gtzeizveqr.html

PHP:  const PI = 3.14159;
来源：http://hz.jyoumei.cn/gtrfdipsud.html

JS:   const PI = 3.14159;
来源：http://hz.fengsongda.top/gtcjlnruuc.html

TS:   const PI: number = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtsbvkonaz.html

Java: static final double PI = 3.14159;
来源：http://hz.pycfn.com/gtwftkpyrq.html

Go:   const PI = 3.14159
来源：http://hz.tian-w.cn/gtqxmqgqfj.html

Ruby: PI = 3.14159
来源：http://hz.bjfxy.top/gthayycaps.html

C#:   const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtpljmmgyp.html

[A04] 判断变量类型
来源：http://hz.iojbl.cn/gtsxhruemm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigfzy.top/gttinqixyj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.haohaochexian.top/gtauwsoewx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.kuanghao11.cn/gttmquegnu.html

TS:   typeof x; x instanceof Date
来源：http://hz.xuetiantiany.cn/gtwdgqwsqj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zdqjudy.top/gteydijopc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuxming.cn/gtihyospkj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shanyushiyangkeji.top/gtqrkgzgci.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgfzy.top/gtbacmixcb.html

[A05] 整数除法与取模
来源：http://hz.cucudq.cn/gttcdkiajv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.havefunace.top/gtnceqcahb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.pycfn.com/gtwwpmwswn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ppjwa.cn/gtwnkfbtur.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jyoumei.cn/gtwfghrwtx.html

Java: 7 / 2; 7 % 2
来源：http://hz.zhongyouzk.top/gtfjqmfyxi.html

Go:   7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtkifrvzdi.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtlavogjwx.html

C#:   7 / 2; 7 % 2
来源：http://hz.yangfankeji.com/gtyiejmqxd.html

[A06] 字符串转数字
来源：http://hz.yj202588.top/gtjptpbwzp.html

Py:   int("42"); float("3.14")
来源：http://hz.chenlongwang.top/gtlkntcjel.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cashguo.top/gtcwzxjsor.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shangyingyoupin.top/gtbhnkvzjr.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.sxryk.cn/gtenzoycqj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jinyuanbaomall.cn/gtzgmrhwvp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zycfv.cn/gtfddvtltg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgufenzy.top/gtiseepnut.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dashuyun.cn/gtxhkhpzav.html

[A07] 数字转字符串
来源：http://hz.wangshuangyany.cn/gtdfvxazip.html

Py:   str(42)
来源：http://hz.0kj1m.cn/gtboqugyxq.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhijiandao.cn/gtobiajogb.html

JS:   String(42); (42).toString()
来源：http://hz.aibaodan.cn/gtjufmcasm.html

TS:   String(42)
来源：http://hz.cdnleiting.top/gticjxwpkb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tanke756.top/gthmognbhk.html

Go:   strconv.Itoa(42)
来源：http://hz.jyoumei.cn/gtbmoeiani.html

Ruby: 42.to_s
来源：http://hz.ppjwa.cn/gtfqoivzfj.html

C#:   42.ToString()
来源：http://hz.yonumen.top/gtmeylohpj.html

[A08] 取整与四舍五入
来源：http://hz.pycfn.com/gtgvsttxfr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.gzhubu.top/gtnogpljmq.html


<!-- 参考信息 -->