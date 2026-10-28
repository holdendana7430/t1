代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.snrcjt.cn/gttumebipn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sufxvd.cn/gtvyxoyklv.html

[U60] PHP：JSON 编解码
来源：http://hz.svipenyu.cn/gtjvfnmpbt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gotoacloud.top/gtauegzdru.html

[U61] PHP：正则
来源：http://hz.svipenyu.cn/gtdqicetjd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtfqrvavpk.html

[U62] PHP：日期对象
来源：http://hz.yanxiufei.cn/gtboyathrw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.fzhhl.top/gtinbstcdp.html

[U63] PHP：文件读写
来源：http://hz.52xcode.cn/gtwogemdhg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhongyouzk.top/gtkbenedpy.html

[U64] PHP：目录遍历
来源：http://hz.316326.xyz/gttnxaiyjt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtkwljafhe.html

[U65] PHP：会话
来源：http://hz.ppjwa.cn/gthqrbvtgw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jianghu66.top/gtkndwfbkv.html

[U66] PHP：设置 Cookie
来源：http://hz.chenjidiqi.icu/gtpfkrinvh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangshuangyany.cn/gttnuycwix.html

[U67] PHP：处理文件上传
来源：http://hz.tian-w.cn/gtjkdkmbim.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgfzy.top/gtordiomuj.html

[U68] PHP：PDO 连接
来源：http://hz.tanke756.top/gtdvhpssxa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pengpengdd.cyou/gtmbybqrqq.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gtulroslmg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.pengpengdd.cyou/gttychrwga.html

[U70] PHP：PDO 事务
来源：http://hz.sufxvd.cn/gtwvjkshpt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jianghu66.top/gtvpovdfdy.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gtzhwdfebb.html

throw new RuntimeException("失败", 500);
来源：http://hz.hfpthk.cn/gtrwhuyjdd.html

[U72] PHP：写错误日志
来源：http://hz.guannengcc.top/gtkymevesl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jyoumei.cn/gtwjwxgyxl.html

[U73] PHP：读取 ini 配置
来源：http://hz.cashguo.top/gtrxrzbnmv.html

parse_ini_file("config.ini", true)
来源：http://hz.shzxlz.cn/gtjhpbuwnq.html

[U74] PHP：读取环境变量
来源：http://hz.haohaochexian.top/gtvhrxghai.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jqgfzy.top/gtehdesbwm.html

[U75] PHP：依赖注入
来源：http://hz.sysykeji.top/gtnahmvbhd.html

composer require psr/container
来源：http://hz.zhoulong.xyz/gtnyjwouip.html

[U76] PHP：简单路由
来源：http://hz.snrcjt.cn/gtyzobzaku.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hywenlv.cn/gtvfncfijt.html

[U77] PHP：模板渲染
来源：http://hz.guannengcc.top/gtwhbbwhkj.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gtwcknelxf.html

[U78] PHP：单元测试
来源：http://hz.mhx1999.top/gtnlpmycmn.html

composer require --dev phpunit/phpunit
来源：http://hz.pycfn.com/gttcyxacik.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtmxmzeveg.html

composer require --dev phpstan/phpstan
来源：http://hz.hysaishi.cn/gtmjjkjjdb.html

[U80] PHP：代码规范修复
来源：http://hz.aizwys.cn/gtaclyumep.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yvedp.cn/gtbluglwav.html

[U81] JS：初始化项目
来源：http://hz.havefunace.top/gtqzguwuem.html

npm init -y;  npm i express
来源：http://hz.yangfankeji.com/gtvxbjlcdd.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gtxfmiwqfh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jqgufenzy.top/gtdrlskcsi.html

[U83] JS：ES Module 导入导出
来源：http://hz.xingfuxueyuan.xyz/gtkwectifr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhengqikj.top/gtkvgnbaxd.html

[U84] JS：CommonJS 写法
来源：http://hz.dashuyun.cn/gtzkvhahrj.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gthotefswb.html

[U85] JS：可选链
来源：http://hz.wangdashe.top/gtfeespugz.html

a?.b?.c
来源：http://hz.xinyue.icu/gtleetumpo.html

[U86] JS：空值合并
来源：http://hz.shuidangran.top/gtqlnrxoxt.html

a ?? b
来源：http://hz.sxryk.cn/gtglvxryve.html

[U87] JS：解构默认值
来源：http://hz.birdmap.top/gtsywjzrir.html

const { a = 1, b = 2 } = obj;
来源：http://hz.svipenyu.cn/gtwqyantnv.html

[U88] JS：对象展开合并
来源：http://hz.jqgufenzy.top/gtoeyaqdmw.html

{ ...a, ...b }
来源：http://hz.pengpengdd.cyou/gtpwjvczxo.html

[U89] JS：数组去重
来源：http://hz.jinyuanbaomall.cn/gtpuxozvwz.html

[...new Set(arr)]
来源：http://hz.xylfe.cn/gtoultytuc.html

[U90] JS：数字数组排序
来源：http://hz.chenzaomai.com/gtfdqeygzf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtrqpffexs.html

[U91] JS：对象键值遍历
来源：http://hz.ybcxt.top/gtbvabuanw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shanyushiyangkeji.top/gtcnqxpagd.html

[U92] JS：深拷贝
来源：http://hz.xziqi.cn/gtlqrkeack.html

structuredClone(obj)
来源：http://hz.hnqzz.top/gtyfvzuxwf.html

[U93] JS：模板字符串
来源：http://hz.wangshuangyany.cn/gtqpjugyer.html

`共 ${n} 条`
来源：http://hz.kuanghao11.cn/gtmsxptsry.html

[U94] JS：箭头函数
来源：http://hz.ydjk.org.cn/gtpcxmadnt.html

const double = x => x * 2;
来源：http://hz.zycfv.cn/gtmjimsdwi.html

[U95] JS：Promise 包装
来源：http://hz.yuanzhike.top/gtbjqkvzwo.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigufen.top/gtmmdytvhi.html

[U96] JS：async/await 与异常
来源：http://hz.shanyushiyangtech.top/gtdlxxkwfx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtofzxgsyu.html

[U97] JS：并发请求
来源：http://hz.hnxiangtu.top/gtseihttlh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtmmemjpfd.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhixingplan.top/gtewlfghug.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gaohongyu789.top/gtxhcsbzgl.html

[U99] JS：事件监听
来源：http://hz.jqgufenzy.top/gtvszwvvgd.html

el.addEventListener("click", e => {})
来源：http://hz.zhaomingkeji.xyz/gtpmhymqek.html

[U100] JS：DOM 查询
来源：http://hz.wangshuangyany.cn/gtaiyhaezh.html

document.querySelector(".item")
来源：http://hz.yuxming.cn/gtyqipjast.html

[U101] JS：classList 操作
来源：http://hz.feifeiyinyue.top/gtvhapnbky.html

el.classList.toggle("active")
来源：http://hz.hywenlv.cn/gteadxwhcg.html

[U102] JS：本地存储
来源：http://hz.jianghu66.top/gtnpkaeqkw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtmvonehxx.html

[U103] JS：定时器
来源：http://hz.yongpay.top/gtvkiemfyj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangtech.top/gtvormfizy.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtnbqcldkz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtovaxhupa.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtpbnrwgmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gtgjnvpdny.html

[U106] JS：日期格式化
来源：http://hz.jianghu66.top/gtvtjwxhpr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuetiantiany.cn/gtgekmovyd.html

[U107] JS：数字千分位
来源：http://hz.jinqigfzy.top/gtaofqskny.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtjtqmrqtt.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtuouorhup.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gtqdvgrqks.html

[U109] JS：数组分组
来源：http://hz.jiagoushi.top/gtaksxooyg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtcyjtxevg.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtmcavekhg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.fengsongda.top/gtqygrckix.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtfqnmsegs.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtavxqgqaq.html

[U112] JS：字符串补位
来源：http://hz.0kj1m.cn/gtyvxbmqdf.html

"7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtcchrzrzp.html

[U113] JS：正则替换全部
来源：http://hz.jiagoushi.top/gtagbqrtmi.html

s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtthzqvtdy.html

[U114] JS：JSON 深比较
来源：http://hz.jlsjyb.cn/gtinynaaio.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtstepvbwv.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gteuqxlork.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtpikqvllw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yuanzhike.top/gtdhsnuwsr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cucudq.cn/gtsxddvfdd.html

[U117] JS：单元测试
来源：http://hz.chenjidiqi.icu/gtmmvcvgkq.html

npm i -D vitest;  npx vitest
来源：http://hz.hnqzz.top/gtfzxinujd.html

[U118] JS：开发服务器
来源：http://hz.fengsongda.top/gtkhiudjyx.html

npm i -D vite;  npx vite
来源：http://hz.zhiwuduotai.top/gtuwvweito.html

[U119] JS：生产构建
来源：http://hz.jinghuilouyu.cn/gtegxizrzd.html

npx vite build
来源：http://hz.kuanghao11.cn/gthxhvctow.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.mhx1999.top/gtsrnsiikj.html

import.meta.env.VITE_API_URL
来源：http://hz.jlsjyb.cn/gtkxjyxsbl.html

================================================================================
来源：http://hz.c1oappe.top/gtchajnavt.html

统计汇总
来源：http://hz.52xcode.cn/gtymfcvtsb.html

================================================================================
来源：http://hz.daxiang520.top/gtyvufuqho.html

按语言统计（条）：
来源：http://hz.hysaishi.cn/gtmuduskmj.html

Python ......... 252
来源：http://hz.yanxiufei.cn/gtidspkgwp.html

PHP ............ 252
来源：http://hz.jinyuanbaomall.cn/gtyaodsgdo.html

JavaScript ..... 252
来源：http://hz.tianlin.xyz/gtivykhxil.html

TypeScript ..... 212
来源：http://hz.mhx1999.top/gtjsakwwih.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtyxdyhqxt.html

Go ............. 212
来源：http://hz.cucudq.cn/gtfvacobjl.html

Ruby ........... 212
来源：http://hz.xylfe.cn/gtfcqseucv.html

C# ............. 212
来源：http://hz.sweek.top/gtlmxkjxej.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gthdedilrh.html

C++ ............ 30
来源：http://hz.shanyushiyangtech.top/gtzqjsovyr.html

SQL ............ 90
来源：http://hz.guowangkeji.top/gtxtpfvxxn.html

Bash ........... 80
来源：http://hz.guowangkeji.top/gtmtdblkoz.html

Kotlin ......... 15
来源：http://hz.kuanghao11.cn/gtdyxvufot.html

Swift .......... 15
来源：http://hz.guowangkeji.top/gtmjvlzfgc.html

Lua ............ 10
来源：http://hz.shuidangran.top/gthqoxviai.html

Perl ........... 10
来源：http://hz.dashuyun.cn/gtmrjandhg.html

Scala .......... 10
来源：http://hz.52xcode.cn/gtmrwdczgm.html

------------------------------------
来源：http://hz.hysaishi.cn/gtyyfqcaih.html

合计 ........... 2106 条
来源：http://hz.jqgfzy.top/gtborlynhh.html

按章节统计：
来源：http://hz.haohaochexian.top/gttiohcjpe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtiedzgzcc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtsnwakjpk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtomhqwvmt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gteynsaafg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jqgufenzy.top/gthtkfljwz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtjaprhlya.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.vqdsnc.cn/gthxcdcplo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yonumen.top/gtujickbdf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gthzneguth.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtvvfvnapv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtwpfjfnwq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gttcimlbjl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gteojdugrj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangkeji.top/gtsexbosdj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cucudq.cn/gtbkfhtghv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtlucmcymc.html

Q SQL 专题                              90
来源：http://hz.0kj1m.cn/gtvtxzrjle.html

R Bash 专题                             80
来源：http://hz.chenzaomai.com/gtkmvfytvz.html

S C / C++ 专题                          60
来源：http://hz.yj20258888.top/gtmnbcuowf.html

T 其他语言补充                          60
来源：http://hz.vqdsnc.cn/gtkrzqrhmj.html

U 高频实用片段                         120
来源：http://hz.zhixingplan.top/gtvcctzfow.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtgifnfcsa.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtlqvqryqg.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gttdfjnksr.html

使用提醒
来源：http://hz.ydjk.org.cn/gtjvzmbnhi.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtdajfjneg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.svipenyu.cn/gtxunubjwp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuanzhike.top/gtldqtrpmx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tian-w.cn/gtavfzxbih.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hysaishi.cn/gtvwvpsmvy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aibaodan.cn/gtyojrtuqa.html

—— 文件结束 ——
来源：http://hz.guowangkeji.top/gtvexwjfhk.html

================================================================================
来源：http://hz.yuanzhike.top/gtpkwgkhgi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nwbrower.top/gtumtinznv.html

Common Programming Examples Cheat Book
来源：http://hz.dashuyun.cn/gtiaxnphzx.html

================================================================================
来源：http://hz.jiagoushi.top/gtgsyifydx.html

【收录内容】
来源：http://hz.hywenlv.cn/gtpzearosf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cashguo.top/gtrejdpdvt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xuetiantiany.cn/gtdxxhwdyx.html

SQL · Bash · C · C++
来源：http://hz.pengpengdd.cyou/gtzaiwdokf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.fzhhl.top/gtzzpktauj.html

【使用说明】
来源：http://hz.aizwys.cn/gtvhrxirgu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ppjwa.cn/gthjlhtqzk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yangfankeji.com/gtncoujfvy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.guannengcc.top/gteudbpaqa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.haohaochexian.top/gtajtlmfjs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.mhx1999.top/gtmmhbqjgh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtggutwpxc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sweek.top/gtwzxhyzpv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigufen.top/gtafvqrmia.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zycfv.cn/gtqtiqnade.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.52xcode.cn/gtbgccxmmg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yuxming.cn/gtlagiipoy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hnxiangtu.top/gthbwtpogk.html

【文件统计】
来源：http://hz.cheryme.top/gtcduucaej.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yongpay.top/gtxgwsveuv.html

--------------------------------------------------------------------------------
来源：http://hz.yangfankeji.com/gtogrekjol.html

目  录
来源：http://hz.yanxiufei.cn/gtgjlpivbm.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtdhpgfrff.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtuiegwjva.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtlvkxemnq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ppjwa.cn/gtwfqkahfc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtmckscxtr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj20258888.top/gtwsjxlanb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtkxkcdvyh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtehnhcpqo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.havefunace.top/gthudxhtzb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gthogskduv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.vqdsnc.cn/gtvxmmesso.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtasmllsnr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gthtmjjogo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtmrgrrzuv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sxryk.cn/gtivyizymo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sxryk.cn/gtwlmknmor.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gttfsrmmsb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zycfv.cn/gtkbopfzla.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fengsongda.top/gtiyfkglvp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shuidangran.top/gtemaeumra.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtywtesjpy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtqytbdrex.html

================================================================================
来源：http://hz.mhx1999.top/gtsmjlmzio.html

A. 基础语法与类型
来源：http://hz.xingfuxueyuan.xyz/gtwnbxmapc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwgkcukig.html

[A01] Hello World
来源：http://hz.aizwys.cn/gtpumfrzyr.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangkeji.top/gtsiyxohiz.html

PHP:  echo "Hello, World!";
来源：http://hz.zhiwuduotai.top/gtkoeebmoz.html

JS:   console.log("Hello, World!");
来源：http://hz.cheryme.top/gtsqmeyknc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zdqjudy.top/gtjihvfewo.html

Java: System.out.println("Hello, World!");
来源：http://hz.zdqjudy.top/gtwdyjeaaq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.tian-w.cn/gtembtltzq.html

Ruby: puts "Hello, World!"
来源：http://hz.fzhhl.top/gtjrnqxvye.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.jinqigfzy.top/gtiwzdhcdz.html

[A02] 变量声明与赋值
来源：http://hz.sufxvd.cn/gtanzoqjup.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.dashuyun.cn/gtkwjdzjyn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhijiandao.cn/gtkwrgssez.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj202588.top/gtzzfzerdp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gtwclchgjb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtwkjoimko.html

Go:   name := "Alex"; age := 20
来源：http://hz.yangfankeji.com/gtcvrxxikn.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yj202588.top/gtsvdnsgbf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhongyouzk.top/gtlvrecmpr.html

[A03] 常量定义
来源：http://hz.wangshuangyany.cn/gttihxsbei.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shanyushiyangtech.top/gtnqsipdor.html

PHP:  const PI = 3.14159;
来源：http://hz.jyoumei.cn/gtxunyoyxe.html

JS:   const PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtmvhexwus.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhoulong.xyz/gtxizikoka.html

Java: static final double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtivvkszcf.html

Go:   const PI = 3.14159
来源：http://hz.yj20258888.top/gtipvkhcyf.html

Ruby: PI = 3.14159
来源：http://hz.hnqzz.top/gtdggfsyvm.html

C#:   const double PI = 3.14159;
来源：http://hz.tanke756.top/gtpjvwttok.html

[A04] 判断变量类型
来源：http://hz.ywan-chungtsiang.top/gtzjwgrrmx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.andypj.xyz/gteahlnukd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.wangshuangyany.cn/gtogjhjblv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.quarkkingdee.top/gtukllhlnd.html

TS:   typeof x; x instanceof Date
来源：http://hz.haohaochexian.top/gtkvygfufb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sufxvd.cn/gtwjesqptu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.chenjidiqi.icu/gtxnzwugkw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xylfe.cn/gtuxubrnpz.html

C#:   x.GetType().Name; x is int
来源：http://hz.quarkkingdee.top/gtikvclzqj.html

[A05] 整数除法与取模
来源：http://hz.bjfxy.top/gtabwdistf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.pengpengdd.cyou/gtrvvgnxso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jlsjyb.cn/gtrxtbhyhj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtnkgeixit.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hongshengwenyu.top/gtolsbtpok.html

Java: 7 / 2; 7 % 2
来源：http://hz.hnqzz.top/gtxsjbduxi.html

Go:   7 / 2; 7 % 2
来源：http://hz.vqdsnc.cn/gtelbeirdb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xylfe.cn/gttbpcmrbc.html

C#:   7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtkjnkfmnc.html

[A06] 字符串转数字
来源：http://hz.haohaochexian.top/gtbujrsmdv.html

Py:   int("42"); float("3.14")
来源：http://hz.cqqwz.cn/gtelvajkmy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.wangshuangyany.cn/gtrxaepfgf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hysaishi.cn/gtnlpmwuth.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xingfuxueyuan.xyz/gtwashwhil.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.0kj1m.cn/gtkhsmidlq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hfpthk.cn/gtmenjrkaf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhongyouzk.top/gtlduxcmmx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xziqi.cn/gtmwvvguff.html

[A07] 数字转字符串
来源：http://hz.gogol.net.cn/gtvzzjbgeq.html

Py:   str(42)
来源：http://hz.xuanzx.com/gtsbhwchjx.html

PHP:  (string) 42; strval(42)
来源：http://hz.gotoacloud.top/gtqidvvtem.html

JS:   String(42); (42).toString()
来源：http://hz.jiagoushi.top/gtkhrhwvkc.html

TS:   String(42)
来源：http://hz.jianghu66.top/gtizjpjwpf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhoulong.xyz/gtmcrcndjk.html

Go:   strconv.Itoa(42)
来源：http://hz.shangyingyoupin.top/gtezjwxtoj.html

Ruby: 42.to_s
来源：http://hz.hnxiangtu.top/gtajxpapbf.html

C#:   42.ToString()
来源：http://hz.jqgfzy.top/gtyrcuwhcg.html

[A08] 取整与四舍五入
来源：http://hz.jiagoushi.top/gtnmuueoor.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shuidangran.top/gtuykufyua.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.snrcjt.cn/gtqlxriwpc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sysykeji.top/gtgglnwpek.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yueranfly.top/gtkieehtjr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.birdmap.top/gtmylbpifn.html


<!-- 参考信息 -->