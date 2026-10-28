代发 wailian999

[U57] PHP：字符串插值
来源：http://hz.meibo888.top/gteenqvacy.html

"值: {$a}"
来源：http://hz.yuanzhike.top/gtfdcokzwh.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtsmallfpp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hysaishi.cn/gtdvkpcvnj.html

[U59] PHP：自定义排序
来源：http://hz.gogol.net.cn/gtclhzdlcz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gtigkaxclm.html

[U60] PHP：JSON 编解码
来源：http://hz.svipenyu.cn/gtovcnlstj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.haohaochexian.top/gtghfcqczd.html

[U61] PHP：正则
来源：http://hz.jinqigfzy.top/gtvtnftphn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtwzlbpbax.html

[U62] PHP：日期对象
来源：http://hz.yj20258888.top/gtdnentgtd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.kuanghao11.cn/gtrgjygzlx.html

[U63] PHP：文件读写
来源：http://hz.ywan-chungtsiang.top/gtcdziygik.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dashuyun.cn/gtalrgzslz.html

[U64] PHP：目录遍历
来源：http://hz.jyoumei.cn/gtkyobteaj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xuetiantiany.cn/gtfrnvohik.html

[U65] PHP：会话
来源：http://hz.iojbl.cn/gtodrclhxt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangshuangyany.cn/gttxfkzzrw.html

[U66] PHP：设置 Cookie
来源：http://hz.tian-w.cn/gtwislwegf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cheryme.top/gthfcxcnxl.html

[U67] PHP：处理文件上传
来源：http://hz.yuanzhike.top/gtsowywows.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.mhx1999.top/gtbeemfuwq.html

[U68] PHP：PDO 连接
来源：http://hz.svipenyu.cn/gtbjymypee.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nwbrower.top/gtlvnqtjps.html

[U69] PHP：PDO 预处理
来源：http://hz.xuetiantiany.cn/gtvpjcjojq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.52xcode.cn/gtuezoszae.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtlgmnnxwk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.0kj1m.cn/gtkadegsvx.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gtdcbzpeuu.html

throw new RuntimeException("失败", 500);
来源：http://hz.svipenyu.cn/gtvgrygrpq.html

[U72] PHP：写错误日志
来源：http://hz.sweek.top/gtnwncxmdu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtwflupald.html

[U73] PHP：读取 ini 配置
来源：http://hz.tianlin.xyz/gthhfskosx.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgufenzy.top/gteauonexc.html

[U74] PHP：读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gteepthvpg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinghuilouyu.cn/gtqcnmscmi.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtkjagwthb.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gtwjlziegn.html

[U76] PHP：简单路由
来源：http://hz.yonumen.top/gtlshooskn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yuxming.cn/gtytqoutxz.html

[U77] PHP：模板渲染
来源：http://hz.jinqigfzy.top/gtpxwqvphz.html

composer require twig/twig
来源：http://hz.zhongyouzk.top/gtdprktbzj.html

[U78] PHP：单元测试
来源：http://hz.chenlongwang.top/gtqdpzdlao.html

composer require --dev phpunit/phpunit
来源：http://hz.jqgufenzy.top/gticggwxxu.html

[U79] PHP：静态分析
来源：http://hz.jinqigufen.top/gtbkxgtcxg.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxuanxn.top/gteavuwthk.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtzckoejoy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xylfe.cn/gtrhdfyuyq.html

[U81] JS：初始化项目
来源：http://hz.jiagoushi.top/gtirgvdtks.html

npm init -y;  npm i express
来源：http://hz.ybcxt.top/gtgeftypzr.html

[U82] JS：package.json 脚本
来源：http://hz.sxryk.cn/gttcjzghma.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.kuanghao11.cn/gtjnnubauj.html

[U83] JS：ES Module 导入导出
来源：http://hz.xuanzx.com/gtkwcuijxk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.feifeiyinyue.top/gthubymxvg.html

[U84] JS：CommonJS 写法
来源：http://hz.yj20258.top/gtciiwftuw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pengpengdd.cyou/gtlpouijas.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtcqidubpu.html

a?.b?.c
来源：http://hz.shuidangran.top/gtryyavfvk.html

[U86] JS：空值合并
来源：http://hz.yonumen.top/gtlzkrtyoo.html

a ?? b
来源：http://hz.nanxuanxn.top/gtqujikyov.html

[U87] JS：解构默认值
来源：http://hz.kuanghao11.cn/gteempnbjb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinghuilouyu.cn/gtahltnavd.html

[U88] JS：对象展开合并
来源：http://hz.yuxming.cn/gtwhiqpktj.html

{ ...a, ...b }
来源：http://hz.xuanzx.com/gtzlcatsan.html

[U89] JS：数组去重
来源：http://hz.zhengqikj.top/gtqtvxvbuz.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtmnkubbqh.html

[U90] JS：数字数组排序
来源：http://hz.ppjwa.cn/gtmrmuelyq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtcppthtor.html

[U91] JS：对象键值遍历
来源：http://hz.jiagoushi.top/gtjerzjjkv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ydjk.org.cn/gtbtpsqpgb.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtoohjpdmr.html

structuredClone(obj)
来源：http://hz.52xcode.cn/gtmcigxfso.html

[U93] JS：模板字符串
来源：http://hz.chenzaomai.com/gtowvshvlx.html

`共 ${n} 条`
来源：http://hz.ybcxt.top/gtcarjqvyk.html

[U94] JS：箭头函数
来源：http://hz.redwolf501.top/gtengngqnj.html

const double = x => x * 2;
来源：http://hz.9152youxi.cn/gtyfiqudib.html

[U95] JS：Promise 包装
来源：http://hz.zhengqikj.top/gtmxjfpaxu.html

new Promise((resolve, reject) => {})
来源：http://hz.birdmap.top/gtnwkxaenj.html

[U96] JS：async/await 与异常
来源：http://hz.ybcxt.top/gtcfnruftq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtfrpbcuvp.html

[U97] JS：并发请求
来源：http://hz.cqqwz.cn/gtfiikrwii.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtarvsritb.html

[U98] JS：fetch 带 JSON
来源：http://hz.c1oappe.top/gtjmmpxhmf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtzoljkayx.html

[U99] JS：事件监听
来源：http://hz.guowangkeji.top/gtfnbimpxj.html

el.addEventListener("click", e => {})
来源：http://hz.shuidangran.top/gtfmdkcdmu.html

[U100] JS：DOM 查询
来源：http://hz.ybcxt.top/gtwquirjzp.html

document.querySelector(".item")
来源：http://hz.yanxiufei.cn/gtibyuryuc.html

[U101] JS：classList 操作
来源：http://hz.xylfe.cn/gtemavyiyq.html

el.classList.toggle("active")
来源：http://hz.aibaodan.cn/gtrefengsa.html

[U102] JS：本地存储
来源：http://hz.yuxming.cn/gtnhhuzkpc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258888.top/gtwhdskaab.html

[U103] JS：定时器
来源：http://hz.sufxvd.cn/gttjppdpde.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtbswosuyg.html

[U104] JS：防抖
来源：http://hz.guowangkeji.top/gtgqypnpeg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtzeyvnrmv.html

[U105] JS：节流
来源：http://hz.aibaodan.cn/gtzbnfbsln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.9152youxi.cn/gtkgxgepie.html

[U106] JS：日期格式化
来源：http://hz.chenzaomai.com/gtnavbrfbv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gzhubu.top/gtzlxvpbto.html

[U107] JS：数字千分位
来源：http://hz.yuanzhike.top/gtkvdorczl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.chenlongwang.top/gtzrkvqmoq.html

[U108] JS：随机整数
来源：http://hz.yj202588.top/gtspurjyvs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258888.top/gtsbxeoboc.html

[U109] JS：数组分组
来源：http://hz.yongpay.top/gtbecfjxpu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtxhznjjxu.html

[U110] JS：数组分块
来源：http://hz.gaohongyu789.top/gtasmefjiv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gaohongyu789.top/gtwsfunnhe.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtsqwuypjv.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gtzlftolhn.html

[U112] JS：字符串补位
来源：http://hz.nwbrower.top/gtfkhylpko.html

"7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtzcclpsoj.html

[U113] JS：正则替换全部
来源：http://hz.316326.xyz/gtcerjrczv.html

s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtazmrzmdw.html

[U114] JS：JSON 深比较
来源：http://hz.nanxuanxn.top/gtlkpegghh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtomrcpmmq.html

[U115] JS：生成 UUID
来源：http://hz.jiagoushi.top/gtvnmcensj.html

crypto.randomUUID()
来源：http://hz.pycfn.com/gtdhhxoeez.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hysaishi.cn/gtusgkjtjb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhixingplan.top/gtsaissglk.html

[U117] JS：单元测试
来源：http://hz.pycfn.com/gtxodrmvga.html

npm i -D vitest;  npx vitest
来源：http://hz.bjfxy.top/gtqubucqjf.html

[U118] JS：开发服务器
来源：http://hz.yongpay.top/gtdnzdlxew.html

npm i -D vite;  npx vite
来源：http://hz.kuanghao11.cn/gteklvsrjp.html

[U119] JS：生产构建
来源：http://hz.guowangkeji.top/gtrsmgzcwo.html

npx vite build
来源：http://hz.shanyushiyangtech.top/gtzhhwaedl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hongshengwenyu.top/gtmkexmmdk.html

import.meta.env.VITE_API_URL
来源：http://hz.tianlin.xyz/gtbgiwitle.html

================================================================================
来源：http://hz.ydzc1.top/gtiqtfsehf.html

统计汇总
来源：http://hz.shanyushiyangtech.top/gtyckpnmcg.html

================================================================================
来源：http://hz.jiagoushi.top/gtztdzgxin.html

按语言统计（条）：
来源：http://hz.jyoumei.cn/gtykohiqgj.html

Python ......... 252
来源：http://hz.xuanzx.com/gtclejrhdb.html

PHP ............ 252
来源：http://hz.316326.xyz/gtehtysapz.html

JavaScript ..... 252
来源：http://hz.havefunace.top/gtwnoqmysr.html

TypeScript ..... 212
来源：http://hz.52xcode.cn/gttumktaoe.html

Java ........... 212
来源：http://hz.xuanzx.com/gtimlrrbow.html

Go ............. 212
来源：http://hz.0kj1m.cn/gtklsptxot.html

Ruby ........... 212
来源：http://hz.chenlongwang.top/gtyxzbbxeh.html

C# ............. 212
来源：http://hz.birdmap.top/gtppwaurcs.html

C .............. 30
来源：http://hz.sufxvd.cn/gtptgzynhc.html

C++ ............ 30
来源：http://hz.quarkkingdee.top/gtjgkmqsrn.html

SQL ............ 90
来源：http://hz.dashuyun.cn/gtdhiayrce.html

Bash ........... 80
来源：http://hz.jqgufenzy.top/gtanpptecn.html

Kotlin ......... 15
来源：http://hz.fzhhl.top/gtqmxpgyfg.html

Swift .......... 15
来源：http://hz.c1oappe.top/gtnbwimzre.html

Lua ............ 10
来源：http://hz.cashguo.top/gtocoocmny.html

Perl ........... 10
来源：http://hz.jlsjyb.cn/gteglkcgbh.html

Scala .......... 10
来源：http://hz.cashguo.top/gtkzsmbnbc.html

------------------------------------
来源：http://hz.zhengqikj.top/gtpkdcrelj.html

合计 ........... 2106 条
来源：http://hz.dianchejie.cn/gtqloiqwai.html

按章节统计：
来源：http://hz.yj20258888.top/gthyrtxgjp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtlymafxxr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gttewgywgg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtealinonl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtdkiauhbv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.daxiang520.top/gtmakuvodu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtdjygmmgl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aibaodan.cn/gtwkyewoiv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtadpnnwpd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtgxxdmzal.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtgiqjnehc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gthcafghke.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtbticffcm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtqbpbocbm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gtzdpslicx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenzaomai.com/gtqngvktjr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtggxukapo.html

Q SQL 专题                              90
来源：http://hz.hnqzz.top/gtbqageelr.html

R Bash 专题                             80
来源：http://hz.meibo888.top/gtfmzermsa.html

S C / C++ 专题                          60
来源：http://hz.52xcode.cn/gteptbgaqk.html

T 其他语言补充                          60
来源：http://hz.yonumen.top/gtvbyoozfx.html

U 高频实用片段                         120
来源：http://hz.zhoulong.xyz/gtodgzfozb.html

------------------------------------
来源：http://hz.smart0.xyz/gtqztiunct.html

合计                                  2106 条
来源：http://hz.chenlongwang.top/gtjldbrnni.html

--------------------------------------------------------------------------------
来源：http://hz.tianlin.xyz/gtnsdvqpyz.html

使用提醒
来源：http://hz.tianlin.xyz/gtkobxwgvm.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtxjckfvkp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtqbweglex.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nanxinkj.top/gtzqwditnw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hongshengwenyu.top/gtwqltghxq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xinyue.icu/gtbgkzhmre.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aizwys.cn/gtydafbkij.html

—— 文件结束 ——
来源：http://hz.snrcjt.cn/gtzqdxpack.html

================================================================================
来源：http://hz.snrcjt.cn/gtmusbngvk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinqigufen.top/gtfvpzshcp.html

Common Programming Examples Cheat Book
来源：http://hz.hfpthk.cn/gtryjycieu.html

================================================================================
来源：http://hz.xuanzx.com/gtemzmvlhs.html

【收录内容】
来源：http://hz.yuanzhike.top/gtqdibnnis.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.sweek.top/gtvtzznalf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ybcxt.top/gtbahktkeb.html

SQL · Bash · C · C++
来源：http://hz.yonumen.top/gtkfnoufzu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.chenjidiqi.icu/gtttjeqcsr.html

【使用说明】
来源：http://hz.jlsjyb.cn/gtvliumcpc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xuanzx.com/gtpfxbzztv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sxryk.cn/gtqfwymieb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xziqi.cn/gtstyzbefd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxinkj.top/gteutycldo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtrfjmwjzf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yongpay.top/gtrxlmploy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtrnqhdmly.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigfzy.top/gtpaqmxecg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.shuidangran.top/gttpvpvmqn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.sufxvd.cn/gtfnqsdqih.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yangfankeji.com/gtelkwjcqv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cheryme.top/gtqttfirio.html

【文件统计】
来源：http://hz.pycfn.com/gtnpznvqab.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yuanzhike.top/gtscsqcrab.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gtmtbriftj.html

目  录
来源：http://hz.xylfe.cn/gtwhcwptae.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtkgexerdf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.kuanghao11.cn/gtelcdkwgh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtwevwyxqv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zdqjudy.top/gtccpksaar.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtheejhkai.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj20258888.top/gtnaueonrm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtroledjqe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtrtleveod.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xinyue.icu/gtigljkrae.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtqjkjyesr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.cdnleiting.top/gtpdaxeekv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gthrylxqcw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtsmrtjfpy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtleyrcnnf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtsimlzxyx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhengqikj.top/gtwoaxbhkt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtdopvrpdc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ywan-chungtsiang.top/gthfrymynj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangtech.top/gttecrbudz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jiagoushi.top/gtrttsbkhz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtybylyool.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtgmbmhmcn.html

================================================================================
来源：http://hz.fzhhl.top/gtxxuqvmad.html

A. 基础语法与类型
来源：http://hz.zhongyouzk.top/gtitsuqjlr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtnnunwfix.html

[A01] Hello World
来源：http://hz.snrcjt.cn/gtxxriphxv.html

Py:   print("Hello, World!")
来源：http://hz.gaohongyu789.top/gtchmbseib.html

PHP:  echo "Hello, World!";
来源：http://hz.tian-w.cn/gtvghwmwgz.html

JS:   console.log("Hello, World!");
来源：http://hz.redwolf501.top/gtgetdxdhk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cqqwz.cn/gtydwrjxbs.html

Java: System.out.println("Hello, World!");
来源：http://hz.gogol.net.cn/gtilzurnpz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xinyue.icu/gtprfrunhy.html

Ruby: puts "Hello, World!"
来源：http://hz.tian-w.cn/gtfjjcdnvp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydjk.org.cn/gthwrqrvsu.html

[A02] 变量声明与赋值
来源：http://hz.xuanzx.com/gtkpiqolva.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.gogol.net.cn/gtkzmnrzqi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aibaodan.cn/gtiovmwrzj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jyoumei.cn/gtenlljpbe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hfpthk.cn/gtjtktechb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.wangdashe.top/gtchotltex.html

Go:   name := "Alex"; age := 20
来源：http://hz.hnqzz.top/gtrqbtnxhs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtatpxnmub.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtoviovema.html

[A03] 常量定义
来源：http://hz.jlsjyb.cn/gtkeawbjwh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pycfn.com/gtvilhench.html

PHP:  const PI = 3.14159;
来源：http://hz.cashguo.top/gtamvfqecq.html

JS:   const PI = 3.14159;
来源：http://hz.haohaochexian.top/gtlhtyuvuz.html

TS:   const PI: number = 3.14159;
来源：http://hz.gaohongyu789.top/gtcmjatbvf.html

Java: static final double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtegizucbo.html

Go:   const PI = 3.14159
来源：http://hz.fengsongda.top/gtducppsap.html

Ruby: PI = 3.14159
来源：http://hz.hnxiangtu.top/gtghcvcwdo.html

C#:   const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtvwzmdwoa.html

[A04] 判断变量类型
来源：http://hz.jinqigufen.top/gtwvzquyaz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.kuanghao11.cn/gtnyptcvpb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yvedp.cn/gtomjboefx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhiwuduotai.top/gtfjbkczrx.html

TS:   typeof x; x instanceof Date
来源：http://hz.snrcjt.cn/gthbgcktsv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pengpengdd.cyou/gtfiuzalqr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuxming.cn/gtvofjzffn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tian-w.cn/gtyshvixtb.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj202588.top/gtvheerglf.html

[A05] 整数除法与取模
来源：http://hz.daria6918.cn/gtmjbtnscy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yangfankeji.com/gtgrzrhoqz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhijiandao.cn/gtmdlrrbzm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.316326.xyz/gtximfkxfz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.quarkkingdee.top/gtiplzfacj.html

Java: 7 / 2; 7 % 2
来源：http://hz.sweek.top/gtderwnxen.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenjidiqi.icu/gtsxlkzwls.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtfqzleydb.html

C#:   7 / 2; 7 % 2
来源：http://hz.ppjwa.cn/gtlqbbbxxi.html

[A06] 字符串转数字
来源：http://hz.zhixingplan.top/gtebyokgvg.html

Py:   int("42"); float("3.14")
来源：http://hz.ydjk.org.cn/gttkjjlkoz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xylfe.cn/gtesjfrnkm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtdndcbybs.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yj202588.top/gtxzjkfdlz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sufxvd.cn/gtqvpieigr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hongshengwenyu.top/gtlzeebiul.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yuanzhike.top/gtxljaaeyc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xinyue.icu/gtixaqexdl.html

[A07] 数字转字符串
来源：http://hz.zhijiandao.cn/gtukwhvdkx.html

Py:   str(42)
来源：http://hz.cucudq.cn/gtmwrktlwy.html

PHP:  (string) 42; strval(42)
来源：http://hz.jlsjyb.cn/gtgmjgsavr.html

JS:   String(42); (42).toString()
来源：http://hz.zycfv.cn/gtmnlfrzkc.html

TS:   String(42)
来源：http://hz.jinghuilouyu.cn/gthlnmwibc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.tanke756.top/gtoahckihg.html

Go:   strconv.Itoa(42)
来源：http://hz.sufxvd.cn/gttmnkumsx.html

Ruby: 42.to_s
来源：http://hz.zhongyouzk.top/gtxlkqzidb.html

C#:   42.ToString()
来源：http://hz.yj20258888.top/gthohwfhvl.html

[A08] 取整与四舍五入
来源：http://hz.xziqi.cn/gtebaztpnq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yangfankeji.com/gtgjonuftq.html


<!-- 参考信息 -->