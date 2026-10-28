代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.yangfankeji.com/gtwnlwkwcb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtbisdcalm.html

[U60] PHP：JSON 编解码
来源：http://hz.c1oappe.top/gtihzlzzst.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gtrcjobhnu.html

[U61] PHP：正则
来源：http://hz.birdmap.top/gtbqvxhbkk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtxnqbemwa.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangkeji.top/gtunklossb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gtvdsjauip.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gtxdwbuiwa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dianchejie.cn/gtkbxrgakt.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gttckjdsma.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aibaodan.cn/gtclgctegb.html

[U65] PHP：会话
来源：http://hz.chenjidiqi.icu/gtobbldrhm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hammf.cn/gtjqebncak.html

[U66] PHP：设置 Cookie
来源：http://hz.mhx1999.top/gtqdklcyjh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zycfv.cn/gtanebvsod.html

[U67] PHP：处理文件上传
来源：http://hz.chenzaomai.com/gtfcqgvpbw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.guannengcc.top/gtdhmnhwlf.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gtgrjooubc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtanvpqakv.html

[U69] PHP：PDO 预处理
来源：http://hz.dashuyun.cn/gtnykjqaja.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.andypj.xyz/gtrlwpeqhv.html

[U70] PHP：PDO 事务
来源：http://hz.wangshuangyany.cn/gtpdpmgukr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ywan-chungtsiang.top/gtduhmzzxj.html

[U71] PHP：抛出异常
来源：http://hz.zycfv.cn/gtvuqlqrjx.html

throw new RuntimeException("失败", 500);
来源：http://hz.pengpengdd.cyou/gtwecyvwxg.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangtech.top/gtjmrhwbyw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ybcxt.top/gtlrhgsbyb.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gtukuihcyx.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtiwwajkfi.html

[U74] PHP：读取环境变量
来源：http://hz.cdnleiting.top/gtponiwwuq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daxiang520.top/gtmmsfhznj.html

[U75] PHP：依赖注入
来源：http://hz.xziqi.cn/gtzjqymefu.html

composer require psr/container
来源：http://hz.meibo888.top/gtvktmhbys.html

[U76] PHP：简单路由
来源：http://hz.quarkkingdee.top/gtconxmdlb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtstlvzbpr.html

[U77] PHP：模板渲染
来源：http://hz.daxiang520.top/gtjlmpbcwj.html

composer require twig/twig
来源：http://hz.yongpay.top/gtdqwwdbgo.html

[U78] PHP：单元测试
来源：http://hz.ivvv.top/gtlccrovge.html

composer require --dev phpunit/phpunit
来源：http://hz.iojbl.cn/gtkxesdojz.html

[U79] PHP：静态分析
来源：http://hz.zhijiandao.cn/gtszctkxok.html

composer require --dev phpstan/phpstan
来源：http://hz.sysykeji.top/gtvetfxyhy.html

[U80] PHP：代码规范修复
来源：http://hz.hammf.cn/gtjcjmshij.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ybcxt.top/gtervoaivx.html

[U81] JS：初始化项目
来源：http://hz.hammf.cn/gtnvdylpwz.html

npm init -y;  npm i express
来源：http://hz.haohaochexian.top/gtzgstxybi.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtpmvqkqhi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jqgufenzy.top/gtlabqlibn.html

[U83] JS：ES Module 导入导出
来源：http://hz.hongshengwenyu.top/gtwzwnytqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.iojbl.cn/gtehdwegvp.html

[U84] JS：CommonJS 写法
来源：http://hz.gogol.net.cn/gtsvppfmhq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.meibo888.top/gtmmeaowiy.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtvocefzui.html

a?.b?.c
来源：http://hz.aibaodan.cn/gtczxjpozq.html

[U86] JS：空值合并
来源：http://hz.chenzaomai.com/gtsyxedasj.html

a ?? b
来源：http://hz.tian-w.cn/gtcicrdqjd.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtpogkhiyb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnqzz.top/gtryxbfogk.html

[U88] JS：对象展开合并
来源：http://hz.zhoulong.xyz/gtegrcodic.html

{ ...a, ...b }
来源：http://hz.jiagoushi.top/gtrojuvadk.html

[U89] JS：数组去重
来源：http://hz.gogol.net.cn/gtkygcqlhk.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtjsoaecfs.html

[U90] JS：数字数组排序
来源：http://hz.jinyuanbaomall.cn/gtzyqsjrwh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtraiensxt.html

[U91] JS：对象键值遍历
来源：http://hz.chenlongwang.top/gtjumoezkn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sxryk.cn/gtitnazklz.html

[U92] JS：深拷贝
来源：http://hz.gotoacloud.top/gtishmfimo.html

structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtmjqimndx.html

[U93] JS：模板字符串
来源：http://hz.cashguo.top/gtiwouqdhx.html

`共 ${n} 条`
来源：http://hz.guannengcc.top/gtjltoadsj.html

[U94] JS：箭头函数
来源：http://hz.pycfn.com/gtsbseuguh.html

const double = x => x * 2;
来源：http://hz.gzhubu.top/gtdkvzudez.html

[U95] JS：Promise 包装
来源：http://hz.hnqzz.top/gtauwwsrvz.html

new Promise((resolve, reject) => {})
来源：http://hz.pycfn.com/gtdwbfabaj.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtiwhewukh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtnupjprsg.html

[U97] JS：并发请求
来源：http://hz.vqdsnc.cn/gtwqfblznh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtquwbaqsu.html

[U98] JS：fetch 带 JSON
来源：http://hz.jqgufenzy.top/gtdvvsiyxk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuxming.cn/gtxtzmeweo.html

[U99] JS：事件监听
来源：http://hz.zhengqikj.top/gtecdtmler.html

el.addEventListener("click", e => {})
来源：http://hz.yonumen.top/gtmqakducs.html

[U100] JS：DOM 查询
来源：http://hz.gaohongyu789.top/gthsxgbpnd.html

document.querySelector(".item")
来源：http://hz.yj20258.top/gteorfqrlb.html

[U101] JS：classList 操作
来源：http://hz.jyoumei.cn/gtwflcklgd.html

el.classList.toggle("active")
来源：http://hz.dashuyun.cn/gtmwefthla.html

[U102] JS：本地存储
来源：http://hz.xinyue.icu/gtfjbmvmyk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.mhx1999.top/gtsrezwcjq.html

[U103] JS：定时器
来源：http://hz.52xcode.cn/gtrtribain.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daria6918.cn/gtvbxvnrkp.html

[U104] JS：防抖
来源：http://hz.cucudq.cn/gtenyrahqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtclqsdaov.html

[U105] JS：节流
来源：http://hz.smart0.xyz/gtmbjsxfny.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.0kj1m.cn/gtaiafftad.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gtwfrjqmsy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.snrcjt.cn/gtgrpzychw.html

[U107] JS：数字千分位
来源：http://hz.mhx1999.top/gtffnynumu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtjnzyrrph.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtkjolccjv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.cdnleiting.top/gtlfrtyzrx.html

[U109] JS：数组分组
来源：http://hz.dashuyun.cn/gtxggvuthp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtkwqegacy.html

[U110] JS：数组分块
来源：http://hz.hongshengwenyu.top/gtfdqpmzux.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sufxvd.cn/gtcbztfxlc.html

[U111] JS：对象转 Map
来源：http://hz.yuanzhike.top/gtrhqnsvfm.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gteapeydaz.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtnlspmzda.html

"7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gttiadynjh.html

[U113] JS：正则替换全部
来源：http://hz.ywan-chungtsiang.top/gtpzlyrzyv.html

s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtpwunkzjr.html

[U114] JS：JSON 深比较
来源：http://hz.ybcxt.top/gtdhqewhmi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtoywoeqgf.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gtuqnouglb.html

crypto.randomUUID()
来源：http://hz.hammf.cn/gttykioncx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.dashuyun.cn/gtdafqdqee.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shanyushiyangtech.top/gtehmctpfn.html

[U117] JS：单元测试
来源：http://hz.yuxming.cn/gtryizvzdd.html

npm i -D vitest;  npx vitest
来源：http://hz.aibaodan.cn/gtlhzuqmid.html

[U118] JS：开发服务器
来源：http://hz.ybcxt.top/gtyihgzlem.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtkxakksip.html

[U119] JS：生产构建
来源：http://hz.316326.xyz/gtjpwiswze.html

npx vite build
来源：http://hz.shangyingyoupin.top/gtjyctvajk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuanzhike.top/gtsmjhxxan.html

import.meta.env.VITE_API_URL
来源：http://hz.jiagoushi.top/gtzyuizflh.html

================================================================================
来源：http://hz.daria6918.cn/gttwaeywob.html

统计汇总
来源：http://hz.ivvv.top/gtmxzjuork.html

================================================================================
来源：http://hz.xylfe.cn/gtevmfikfr.html

按语言统计（条）：
来源：http://hz.feifeiyinyue.top/gtfxmuhptj.html

Python ......... 252
来源：http://hz.nanxinkj.top/gtjtioaqij.html

PHP ............ 252
来源：http://hz.vqdsnc.cn/gtbyfyatfr.html

JavaScript ..... 252
来源：http://hz.smart0.xyz/gtpsgalqta.html

TypeScript ..... 212
来源：http://hz.zhijiandao.cn/gtybmrdohp.html

Java ........... 212
来源：http://hz.yj202588.top/gtiavigwwf.html

Go ............. 212
来源：http://hz.aizwys.cn/gthfolputd.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtfevcgiyt.html

C# ............. 212
来源：http://hz.xuetiantiany.cn/gtafefqosz.html

C .............. 30
来源：http://hz.yongpay.top/gthyaufmtt.html

C++ ............ 30
来源：http://hz.wangdashe.top/gtrihfzmyg.html

SQL ............ 90
来源：http://hz.shuidangran.top/gtdkdtszmm.html

Bash ........... 80
来源：http://hz.gotoacloud.top/gtrpeeqneu.html

Kotlin ......... 15
来源：http://hz.hnqzz.top/gtbegpawji.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtqignogjs.html

Lua ............ 10
来源：http://hz.yongpay.top/gtlnilonbu.html

Perl ........... 10
来源：http://hz.shangyingyoupin.top/gtqxnfjpde.html

Scala .......... 10
来源：http://hz.havefunace.top/gthupfqyha.html

------------------------------------
来源：http://hz.gaohongyu789.top/gtqsupligx.html

合计 ........... 2106 条
来源：http://hz.xuanzx.com/gtzhonysvv.html

按章节统计：
来源：http://hz.yongpay.top/gttfatxqob.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtbnsjldyb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtmumdvjqh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtyexfqdhe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtsheiaznl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nwbrower.top/gtwlzgldir.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtfysowokw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtlxwmbkce.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hnqzz.top/gtdvrkdjmw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtgwdpptic.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtnkhymanw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtmbcpfxai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtugtkhlss.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtzxlyoopv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtafzwkixb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gtjhnicfbs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtkvtaatii.html

Q SQL 专题                              90
来源：http://hz.fengsongda.top/gtxxmmsopg.html

R Bash 专题                             80
来源：http://hz.havefunace.top/gtjxnpbobv.html

S C / C++ 专题                          60
来源：http://hz.meibo888.top/gtdyllatix.html

T 其他语言补充                          60
来源：http://hz.yuanzhike.top/gtjyuideml.html

U 高频实用片段                         120
来源：http://hz.yj20258888.top/gtdxqtfgfh.html

------------------------------------
来源：http://hz.sufxvd.cn/gtrmctvsda.html

合计                                  2106 条
来源：http://hz.dashuyun.cn/gthtmoaiin.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtvmisplov.html

使用提醒
来源：http://hz.jiagoushi.top/gtgidotqmn.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtugcwwogv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ywan-chungtsiang.top/gthjinttiy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.aibaodan.cn/gtqsfpsgnj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhijiandao.cn/gtigpktutg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj20258.top/gtrobvgjsa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shzxlz.cn/gtkvtpklip.html

—— 文件结束 ——
来源：http://hz.fzhhl.top/gtbvrgghfw.html

================================================================================
来源：http://hz.hnqzz.top/gtqbcsxazj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.birdmap.top/gtjcqqblhb.html

Common Programming Examples Cheat Book
来源：http://hz.ppjwa.cn/gtejshysmy.html

================================================================================
来源：http://hz.ehwqpu.com/gtaclnfncb.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gtptvshjfv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenlongwang.top/gtwipzwlbn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.pycfn.com/gtnpqgiuhc.html

SQL · Bash · C · C++
来源：http://hz.kuanghao11.cn/gtkytwbnzb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinqigfzy.top/gtokseujum.html

【使用说明】
来源：http://hz.yueranfly.top/gtauzjupcr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daria6918.cn/gtfyhxwkio.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ppjwa.cn/gtykusmfxp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gtidasbmde.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtshwmgdgk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ivvv.top/gtmdfffdoh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xziqi.cn/gtfwfigwbl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zycfv.cn/gtahipdeun.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jlsjyb.cn/gtyzpopukk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnxiangtu.top/gtqovzlune.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zycfv.cn/gtexzvcuee.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sysykeji.top/gtmlldiumj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhaomingkeji.xyz/gtqfuqffvs.html

【文件统计】
来源：http://hz.quarkkingdee.top/gtcfdhmkai.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ivvv.top/gtsnkdyexm.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtaxuxaqht.html

目  录
来源：http://hz.redwolf501.top/gtqffnlsrh.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtkuwcpujd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yangfankeji.com/gtwhityolk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xziqi.cn/gtolyzsbsx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtxcfwjucz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.iojbl.cn/gtlnuewjmu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cdnleiting.top/gtxblrkdwc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shanyushiyangkeji.top/gtmzgudazf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gttwytjhqd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gtcocryuww.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gthqqqondf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtlgcywuqr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtccodavuk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtnsequbfr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtpmkjmhxc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gtgqavyjst.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aizwys.cn/gtlueayriw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gttplqqnvg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtsfpwpjlu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtgngtgxie.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hammf.cn/gtsdqdnxaq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtzijwcnhf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtrcdqdntm.html

================================================================================
来源：http://hz.zhengqikj.top/gtjgybquqb.html

A. 基础语法与类型
来源：http://hz.jianghu66.top/gtyftjfukp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzjmlutmf.html

[A01] Hello World
来源：http://hz.xinyue.icu/gtdhaqwyrk.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtaepnvzcf.html

PHP:  echo "Hello, World!";
来源：http://hz.c1oappe.top/gtazzmxvum.html

JS:   console.log("Hello, World!");
来源：http://hz.meibo888.top/gticqebect.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jlsjyb.cn/gtyfjanzvk.html

Java: System.out.println("Hello, World!");
来源：http://hz.nwbrower.top/gtynuwmeep.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.vqdsnc.cn/gthmstuveb.html

Ruby: puts "Hello, World!"
来源：http://hz.shuidangran.top/gtrlktjmwc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gzhubu.top/gtyazezmll.html

[A02] 变量声明与赋值
来源：http://hz.yanxiufei.cn/gtymajxhka.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.smart0.xyz/gtuljmgwts.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yangfankeji.com/gtpwtstwmd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sysykeji.top/gtxfjrhhvl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hongshengwenyu.top/gtakymusnx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.c1oappe.top/gtuxbrggil.html

Go:   name := "Alex"; age := 20
来源：http://hz.hnqzz.top/gtsbscmfem.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cheryme.top/gtrgvrccby.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtnptqevta.html

[A03] 常量定义
来源：http://hz.redwolf501.top/gtivyygpek.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yueranfly.top/gtdqbnrsfm.html

PHP:  const PI = 3.14159;
来源：http://hz.cdnleiting.top/gtmbcmieir.html

JS:   const PI = 3.14159;
来源：http://hz.zhengqikj.top/gtabzuwvdo.html

TS:   const PI: number = 3.14159;
来源：http://hz.dashuyun.cn/gtzzmbnxkx.html

Java: static final double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtscjxmspi.html

Go:   const PI = 3.14159
来源：http://hz.tianlin.xyz/gtbjkystfx.html

Ruby: PI = 3.14159
来源：http://hz.zhongyouzk.top/gtgcwyntam.html

C#:   const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtizjzwoxq.html

[A04] 判断变量类型
来源：http://hz.mhx1999.top/gtkkuozzrc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jqgfzy.top/gtbprfboty.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.pengpengdd.cyou/gtkdnlxips.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.nwbrower.top/gtrlvxngrp.html

TS:   typeof x; x instanceof Date
来源：http://hz.tanke756.top/gtorwjcojj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhixingplan.top/gthclnadtf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zycfv.cn/gtwbjediun.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tianlin.xyz/gtpjbpdihq.html

C#:   x.GetType().Name; x is int
来源：http://hz.chenjidiqi.icu/gtfeudauhs.html

[A05] 整数除法与取模
来源：http://hz.tanke756.top/gtrrivcpxf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.mhx1999.top/gtblqxtylh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cqqwz.cn/gtjvtxthqd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.bjfxy.top/gtpffnhrwl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhixingplan.top/gtpnyolszx.html

Java: 7 / 2; 7 % 2
来源：http://hz.yj20258888.top/gtmxwjyszo.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtlvanznio.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.bjfxy.top/gttjjosmyb.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhixingplan.top/gtxqffivrr.html

[A06] 字符串转数字
来源：http://hz.xinyue.icu/gtlqubfdth.html

Py:   int("42"); float("3.14")
来源：http://hz.zhixingplan.top/gtjwwtrevw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yanxiufei.cn/gtnafrcdor.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtwaqjfwhh.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zycfv.cn/gtlutzbpxd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.mhx1999.top/gtyoekywpz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtvkloqftm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yj20258.top/gtrktlmmrx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cdnleiting.top/gtlyapwref.html

[A07] 数字转字符串
来源：http://hz.gogol.net.cn/gtukufajcg.html

Py:   str(42)
来源：http://hz.jinqigfzy.top/gtpadtozcf.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhaomingkeji.xyz/gtlykipnth.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangkeji.top/gteypjcafj.html

TS:   String(42)
来源：http://hz.yangfankeji.com/gtjerltgsz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.316326.xyz/gtxxyztbwr.html

Go:   strconv.Itoa(42)
来源：http://hz.gotoacloud.top/gtsqsobwjt.html

Ruby: 42.to_s
来源：http://hz.shangyingyoupin.top/gtlxjpotmx.html

C#:   42.ToString()
来源：http://hz.aibaodan.cn/gtddptjcnk.html

[A08] 取整与四舍五入
来源：http://hz.shuidangran.top/gtdojqndvj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cheryme.top/gtxpyemasv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhijiandao.cn/gtkzbccrdf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.guannengcc.top/gtmwiarwmb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhixingplan.top/gtycwhvbrz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.redwolf501.top/gtjbjfmtmi.html


<!-- 参考信息 -->