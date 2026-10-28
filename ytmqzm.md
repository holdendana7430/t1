代发 wailian999

[U63] PHP：文件读写
来源：http://hz.svipenyu.cn/gteneytzri.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtrqbbknof.html

[U64] PHP：目录遍历
来源：http://hz.yangfankeji.com/gtuymkdzaz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtgzfnljzt.html

[U65] PHP：会话
来源：http://hz.wangshuangyany.cn/gtifpweqgw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhaomingkeji.xyz/gteuogcxfl.html

[U66] PHP：设置 Cookie
来源：http://hz.yj202588.top/gtogozjjix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shuidangran.top/gtguqxdqga.html

[U67] PHP：处理文件上传
来源：http://hz.ehwqpu.com/gtwtmrfwtq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nwbrower.top/gtnuqrqwqu.html

[U68] PHP：PDO 连接
来源：http://hz.zycfv.cn/gtxlyeofui.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hywenlv.cn/gtpxffddnn.html

[U69] PHP：PDO 预处理
来源：http://hz.tian-w.cn/gtqkzrnewt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hysaishi.cn/gtuftusfpr.html

[U70] PHP：PDO 事务
来源：http://hz.yongpay.top/gtyiavvzul.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuetiantiany.cn/gtoaqhihxv.html

[U71] PHP：抛出异常
来源：http://hz.hammf.cn/gtklksmrnq.html

throw new RuntimeException("失败", 500);
来源：http://hz.pengpengdd.cyou/gtinytschx.html

[U72] PHP：写错误日志
来源：http://hz.xingfuxueyuan.xyz/gtnzhumzrx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinghuilouyu.cn/gtnrrgivqe.html

[U73] PHP：读取 ini 配置
来源：http://hz.daxiang520.top/gtpeboxflt.html

parse_ini_file("config.ini", true)
来源：http://hz.gzhubu.top/gtohcijxgp.html

[U74] PHP：读取环境变量
来源：http://hz.ydzc1.top/gtawvdpciu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hfpthk.cn/gtlvdnhgbc.html

[U75] PHP：依赖注入
来源：http://hz.hnqzz.top/gtsmgnowlu.html

composer require psr/container
来源：http://hz.yuanzhike.top/gtlbktnukf.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtlhpzuehg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hywenlv.cn/gtkqnykksi.html

[U77] PHP：模板渲染
来源：http://hz.chenjidiqi.icu/gtzaamftpp.html

composer require twig/twig
来源：http://hz.jqgfzy.top/gtjfegrjhk.html

[U78] PHP：单元测试
来源：http://hz.sysykeji.top/gtaqdloiwu.html

composer require --dev phpunit/phpunit
来源：http://hz.fzhhl.top/gtgbtdjtim.html

[U79] PHP：静态分析
来源：http://hz.zhoulong.xyz/gtmoeioket.html

composer require --dev phpstan/phpstan
来源：http://hz.jianghu66.top/gtlnfrienn.html

[U80] PHP：代码规范修复
来源：http://hz.xinyue.icu/gtycrqebvd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hnxiangtu.top/gtwiwhxlbc.html

[U81] JS：初始化项目
来源：http://hz.ywan-chungtsiang.top/gtjiualvlv.html

npm init -y;  npm i express
来源：http://hz.yonumen.top/gtubkicncc.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gttnxcqkys.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yvedp.cn/gtlmmyenwm.html

[U83] JS：ES Module 导入导出
来源：http://hz.yueranfly.top/gtvoqjxekz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gtnpbqttcs.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtlnboxple.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.c1oappe.top/gtthxtvjsj.html

[U85] JS：可选链
来源：http://hz.ydjk.org.cn/gtofeaqnft.html

a?.b?.c
来源：http://hz.mhx1999.top/gtolarledf.html

[U86] JS：空值合并
来源：http://hz.ybcxt.top/gtsmzzxmco.html

a ?? b
来源：http://hz.pycfn.com/gtiunuahwy.html

[U87] JS：解构默认值
来源：http://hz.tanke756.top/gtrztxjdzy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj202588.top/gtzmyhdonj.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtlqswsvdf.html

{ ...a, ...b }
来源：http://hz.pycfn.com/gtydbhujea.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gtpoqdptxn.html

[...new Set(arr)]
来源：http://hz.mhx1999.top/gtvuqtszqj.html

[U90] JS：数字数组排序
来源：http://hz.316326.xyz/gtatllkakd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtudeqkflm.html

[U91] JS：对象键值遍历
来源：http://hz.aibaodan.cn/gthqzcobby.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.havefunace.top/gtroityytw.html

[U92] JS：深拷贝
来源：http://hz.yongpay.top/gtakccdgdb.html

structuredClone(obj)
来源：http://hz.zdqjudy.top/gtftsawbkd.html

[U93] JS：模板字符串
来源：http://hz.hnqzz.top/gthvvfumeu.html

`共 ${n} 条`
来源：http://hz.aizwys.cn/gtkkhzlmzq.html

[U94] JS：箭头函数
来源：http://hz.andypj.xyz/gteehoeyxs.html

const double = x => x * 2;
来源：http://hz.yvedp.cn/gtvcxqioig.html

[U95] JS：Promise 包装
来源：http://hz.jinqigufen.top/gtknahtkzs.html

new Promise((resolve, reject) => {})
来源：http://hz.yanxiufei.cn/gtylyfbhcd.html

[U96] JS：async/await 与异常
来源：http://hz.yuanzhike.top/gtmfwwjslz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtxaakgyms.html

[U97] JS：并发请求
来源：http://hz.hnqzz.top/gtceqmuksm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtlluktlwa.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhijiandao.cn/gtijrpdyef.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gtelofeewe.html

[U99] JS：事件监听
来源：http://hz.sxryk.cn/gtvozrexxe.html

el.addEventListener("click", e => {})
来源：http://hz.cdnleiting.top/gthffjfqvn.html

[U100] JS：DOM 查询
来源：http://hz.cheryme.top/gtwmhcoill.html

document.querySelector(".item")
来源：http://hz.cashguo.top/gtemyafxeu.html

[U101] JS：classList 操作
来源：http://hz.gotoacloud.top/gtsyzpsbze.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtmfgcynkz.html

[U102] JS：本地存储
来源：http://hz.daxiang520.top/gtarhxhagw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xingfuxueyuan.xyz/gtocjkifch.html

[U103] JS：定时器
来源：http://hz.cashguo.top/gtrniizuut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ybcxt.top/gtsgkyztqz.html

[U104] JS：防抖
来源：http://hz.ydjk.org.cn/gtevpftrok.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtwdiikyhg.html

[U105] JS：节流
来源：http://hz.tianlin.xyz/gtrojoovjm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.0kj1m.cn/gtzxfemzgu.html

[U106] JS：日期格式化
来源：http://hz.chenjidiqi.icu/gtfiobrnaz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gtgbzfniqp.html

[U107] JS：数字千分位
来源：http://hz.smart0.xyz/gtpepencve.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.mhx1999.top/gtkiuywavn.html

[U108] JS：随机整数
来源：http://hz.jianghu66.top/gtylgibikk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yanxiufei.cn/gtgqogmqwu.html

[U109] JS：数组分组
来源：http://hz.birdmap.top/gtvqrcdpiy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gtsiwvocge.html

[U110] JS：数组分块
来源：http://hz.shzxlz.cn/gtcoxintqh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xingfuxueyuan.xyz/gtfortlgzk.html

[U111] JS：对象转 Map
来源：http://hz.redwolf501.top/gtvqzsqltt.html

new Map(Object.entries(obj))
来源：http://hz.smart0.xyz/gtjkdsjwvv.html

[U112] JS：字符串补位
来源：http://hz.xuanzx.com/gteqisotee.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtyldhbhcy.html

[U113] JS：正则替换全部
来源：http://hz.wangshuangyany.cn/gtqwzqomfs.html

s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtgvpqpwur.html

[U114] JS：JSON 深比较
来源：http://hz.yuxming.cn/gtuafrorkl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtyzznjuxk.html

[U115] JS：生成 UUID
来源：http://hz.pycfn.com/gtpodibbcr.html

crypto.randomUUID()
来源：http://hz.xylfe.cn/gtrnuptxbj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.daxiang520.top/gtkheflqaf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.havefunace.top/gtztcvbukv.html

[U117] JS：单元测试
来源：http://hz.meibo888.top/gtnldqludl.html

npm i -D vitest;  npx vitest
来源：http://hz.hywenlv.cn/gtbpjiizni.html

[U118] JS：开发服务器
来源：http://hz.birdmap.top/gthpctxwsw.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtbtjigcdb.html

[U119] JS：生产构建
来源：http://hz.sweek.top/gtlklxyfsr.html

npx vite build
来源：http://hz.ydzc1.top/gtdpkbsnqb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.52xcode.cn/gttbuvjqmk.html

import.meta.env.VITE_API_URL
来源：http://hz.ydjk.org.cn/gtfpaejmrp.html

================================================================================
来源：http://hz.jianghu66.top/gtepbvvqbf.html

统计汇总
来源：http://hz.cashguo.top/gtfyedseaz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttltztgss.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtwdruiamf.html

Python ......... 252
来源：http://hz.jianghu66.top/gtoegcxoek.html

PHP ............ 252
来源：http://hz.yj202588.top/gtkwoqzaje.html

JavaScript ..... 252
来源：http://hz.hysaishi.cn/gthmmtixfh.html

TypeScript ..... 212
来源：http://hz.shanyushiyangkeji.top/gtzuzbpwhi.html

Java ........... 212
来源：http://hz.xziqi.cn/gtvdtnzfow.html

Go ............. 212
来源：http://hz.ehwqpu.com/gtcgmopqfa.html

Ruby ........... 212
来源：http://hz.birdmap.top/gtilzfelfk.html

C# ............. 212
来源：http://hz.jqgufenzy.top/gtanozgzsn.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtophdkbbg.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtuctqstdl.html

SQL ............ 90
来源：http://hz.pengpengdd.cyou/gtunhvrhbq.html

Bash ........... 80
来源：http://hz.snrcjt.cn/gtnadoqzmn.html

Kotlin ......... 15
来源：http://hz.zdqjudy.top/gtlnxkmqyv.html

Swift .......... 15
来源：http://hz.zhengqikj.top/gtowruyyhx.html

Lua ............ 10
来源：http://hz.yj20258.top/gtlofxtyoh.html

Perl ........... 10
来源：http://hz.jianghu66.top/gttwmtvujx.html

Scala .......... 10
来源：http://hz.meibo888.top/gtoaayegek.html

------------------------------------
来源：http://hz.jianghu66.top/gtqanlwdpo.html

合计 ........... 2106 条
来源：http://hz.kuanghao11.cn/gtvbonbcjd.html

按章节统计：
来源：http://hz.shangyingyoupin.top/gtmhjzczvz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtcyrpjwjj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtsfntugpa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtksvmpixw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtdetudemq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gthyhackza.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gtbadomesp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtvtvpfezw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtpwtuflta.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gthaflrsgm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtlbgabtif.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtcfxdsgwx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtywowpcoc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtjchtfbiy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtmammhrpj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daxiang520.top/gtqosaoybo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtldfhodtg.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gtttqrjiwi.html

R Bash 专题                             80
来源：http://hz.yonumen.top/gtvvopcrxk.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangkeji.top/gtsztdjube.html

T 其他语言补充                          60
来源：http://hz.chenjidiqi.icu/gtkihgwqvb.html

U 高频实用片段                         120
来源：http://hz.snrcjt.cn/gtdxlwlini.html

------------------------------------
来源：http://hz.aizwys.cn/gtevjdbwpp.html

合计                                  2106 条
来源：http://hz.gogol.net.cn/gtnstjyzbr.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gtphhqwqpk.html

使用提醒
来源：http://hz.jiagoushi.top/gtqbnwptlj.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtxaghjvgg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ehwqpu.com/gtednirxbn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhoulong.xyz/gtkezpqygj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aizwys.cn/gtpcnwgmkp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.svipenyu.cn/gtjkvykehq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.feifeiyinyue.top/gtqafskgag.html

—— 文件结束 ——
来源：http://hz.jinqigfzy.top/gtivgnbsje.html

================================================================================
来源：http://hz.yj20258.top/gtyuqmjlgb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.svipenyu.cn/gtubugqsql.html

Common Programming Examples Cheat Book
来源：http://hz.yuanzhike.top/gtpzkbionq.html

================================================================================
来源：http://hz.yuanzhike.top/gtsgknvqkz.html

【收录内容】
来源：http://hz.cqqwz.cn/gtgwxwvdpb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nanxinkj.top/gtsqwybqae.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ppjwa.cn/gtaagcqgor.html

SQL · Bash · C · C++
来源：http://hz.52xcode.cn/gtchsmbluf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shanyushiyangtech.top/gtvuuhyjhf.html

【使用说明】
来源：http://hz.ivvv.top/gttcywyyae.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nanxinkj.top/gthpraceuu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258888.top/gtmljxedma.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xingfuxueyuan.xyz/gtsxuhphgb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.iojbl.cn/gtjibnqagt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhoulong.xyz/gtkgpwfrle.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sufxvd.cn/gtxnqauejp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gtobtmwtzm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xylfe.cn/gtqurmadrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.daxiang520.top/gtgjmxbyeb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhiwuduotai.top/gttqrtflxh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shuidangran.top/gtgfnxanbz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.svipenyu.cn/gtjtiglcxn.html

【文件统计】
来源：http://hz.shanyushiyangkeji.top/gtkuybrikc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj20258888.top/gtdwwntwya.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtxgsrjspv.html

目  录
来源：http://hz.ivvv.top/gtbymlbfgb.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtdvzjdchb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtnnitbjsv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtpajmlckl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtbgcljsqw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtyyorjgpb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.meibo888.top/gtocgqosmi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtevigipia.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtpgpwxxag.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.andypj.xyz/gtwketmfex.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtlshwtnmm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgfzy.top/gtzlwkchop.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtpxxdtvah.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtrkrcehyv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtpjaqkbie.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hammf.cn/gtqjthvdwm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dianchejie.cn/gthblnikpp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtfuvogydd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sufxvd.cn/gtviopuucb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtxzogslai.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cqqwz.cn/gtyzpvkfib.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtgqfgnhuo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtfhpbdugv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrvsbcvpt.html

A. 基础语法与类型
来源：http://hz.jianghu66.top/gtmyzaikwo.html

================================================================================
来源：http://hz.yongpay.top/gtejldpolv.html

[A01] Hello World
来源：http://hz.hnxiangtu.top/gtjswvmkib.html

Py:   print("Hello, World!")
来源：http://hz.wangdashe.top/gtmbjjvyuk.html

PHP:  echo "Hello, World!";
来源：http://hz.ehwqpu.com/gtlnkcddea.html

JS:   console.log("Hello, World!");
来源：http://hz.guannengcc.top/gtfkbcztif.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhijiandao.cn/gtaxcjocup.html

Java: System.out.println("Hello, World!");
来源：http://hz.cheryme.top/gtxkkunjdr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xylfe.cn/gtunxtuqgp.html

Ruby: puts "Hello, World!"
来源：http://hz.jinghuilouyu.cn/gtmrjtobpy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtucyadodd.html

[A02] 变量声明与赋值
来源：http://hz.xziqi.cn/gtdtyafeuh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.fengsongda.top/gtdvcpkzoy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hammf.cn/gtzhnjlyxw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtjcnatoxj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.chenzaomai.com/gtnopsslnv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gteojmcmlu.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhoulong.xyz/gtqxeordyq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigfzy.top/gtltodknhd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtqhxrmqmp.html

[A03] 常量定义
来源：http://hz.mhx1999.top/gtcfnymgvx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zycfv.cn/gtddhvdpme.html

PHP:  const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtgpjzlrbu.html

JS:   const PI = 3.14159;
来源：http://hz.zhixingplan.top/gtbzhwoubh.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhijiandao.cn/gtcibzrjen.html

Java: static final double PI = 3.14159;
来源：http://hz.iojbl.cn/gtuuvxypxl.html

Go:   const PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtfhgfhqzo.html

Ruby: PI = 3.14159
来源：http://hz.zhixingplan.top/gtiqufexwj.html

C#:   const double PI = 3.14159;
来源：http://hz.ivvv.top/gtmladezgp.html

[A04] 判断变量类型
来源：http://hz.c1oappe.top/gtdhgnigzg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hysaishi.cn/gtlktictbz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.dianchejie.cn/gtrxkwbpxh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.aibaodan.cn/gtdfygwlen.html

TS:   typeof x; x instanceof Date
来源：http://hz.ybcxt.top/gtcvgomibu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jyoumei.cn/gtksqnjagy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj202588.top/gtwigacxap.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.smart0.xyz/gtidcsknrn.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtsxlxvtdl.html

[A05] 整数除法与取模
来源：http://hz.shuidangran.top/gtswdskjeo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.zycfv.cn/gtswghursy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.havefunace.top/gtrqwqltlp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ydzc1.top/gtxwauyjfx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tian-w.cn/gtcljxobtv.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinqigfzy.top/gtgkqygiyb.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtxgrvjksj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ivvv.top/gtpitsmhjd.html

C#:   7 / 2; 7 % 2
来源：http://hz.yanxiufei.cn/gtlfpazofe.html

[A06] 字符串转数字
来源：http://hz.dianchejie.cn/gtisovapkk.html

Py:   int("42"); float("3.14")
来源：http://hz.hnqzz.top/gtmqwyspvj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhongyouzk.top/gtxxapgifv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nanxuanxn.top/gttninfhbj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yanxiufei.cn/gtseyscnvx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jlsjyb.cn/gtafzvtfsy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhijiandao.cn/gtkvhoohvt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgufenzy.top/gtnbguxoqc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shangyingyoupin.top/gtkstvonsh.html

[A07] 数字转字符串
来源：http://hz.ybcxt.top/gtdwfozixu.html

Py:   str(42)
来源：http://hz.cheryme.top/gtoucybsvu.html

PHP:  (string) 42; strval(42)
来源：http://hz.cheryme.top/gtltguhnpx.html

JS:   String(42); (42).toString()
来源：http://hz.tian-w.cn/gthxukznok.html

TS:   String(42)
来源：http://hz.havefunace.top/gtzwhezzkk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yongpay.top/gtpqkykoez.html

Go:   strconv.Itoa(42)
来源：http://hz.zhengqikj.top/gtpuvljzna.html

Ruby: 42.to_s
来源：http://hz.guannengcc.top/gtkmavubbk.html

C#:   42.ToString()
来源：http://hz.chenzaomai.com/gtgouqjafu.html

[A08] 取整与四舍五入
来源：http://hz.zhongyouzk.top/gtjheufuav.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.tian-w.cn/gtawhzmftz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.birdmap.top/gtqxzraqcc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtfmxyrelp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinyuanbaomall.cn/gtcyvohpte.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.svipenyu.cn/gttidcloln.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhiwuduotai.top/gtxqjntawy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.andypj.xyz/gtaktbklwv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.iojbl.cn/gtnxwrtcng.html

[A09] 绝对值与最大最小值
来源：http://hz.gotoacloud.top/gteuribacj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.meibo888.top/gtjtonawjz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258.top/gtkumcxlaw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.9152youxi.cn/gtcpkslbkc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cqqwz.cn/gtrjgresqo.html


<!-- 参考信息 -->