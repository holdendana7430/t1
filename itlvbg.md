代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.ehwqpu.com/gtdlaoxwgv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtfymyvfqy.html

[U60] PHP：JSON 编解码
来源：http://hz.xziqi.cn/gtnztwrekg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sufxvd.cn/gtneddkeaf.html

[U61] PHP：正则
来源：http://hz.ehwqpu.com/gtzkwuqhjb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtmxirhnbq.html

[U62] PHP：日期对象
来源：http://hz.yanxiufei.cn/gtxhwuiyry.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ivvv.top/gtnrvlbsju.html

[U63] PHP：文件读写
来源：http://hz.ydjk.org.cn/gtlaxqvxwp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtmunxyvaa.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtgajdogeo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ywan-chungtsiang.top/gtfnrarbwv.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtaceqwbra.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.daria6918.cn/gtbijysnzp.html

[U66] PHP：设置 Cookie
来源：http://hz.chenlongwang.top/gtvgkzfcsl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangshuangyany.cn/gtsrssalte.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gtjurbrkrs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.sufxvd.cn/gtenzdsusk.html

[U68] PHP：PDO 连接
来源：http://hz.ybcxt.top/gtrhoqmlas.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.fengsongda.top/gtklzotkfi.html

[U69] PHP：PDO 预处理
来源：http://hz.smart0.xyz/gttiqopwuf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.0kj1m.cn/gtrmweyyxt.html

[U70] PHP：PDO 事务
来源：http://hz.316326.xyz/gtggbsfrvv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenjidiqi.icu/gttpagcrju.html

[U71] PHP：抛出异常
来源：http://hz.ybcxt.top/gtehhixhmn.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtltllfszn.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gtembrkopg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtlghtaxnu.html

[U73] PHP：读取 ini 配置
来源：http://hz.nwbrower.top/gtfdixqgvq.html

parse_ini_file("config.ini", true)
来源：http://hz.birdmap.top/gtopxnsbmx.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtmkveiqdr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.9152youxi.cn/gtcmvjsafb.html

[U75] PHP：依赖注入
来源：http://hz.yj202588.top/gtesgkjayy.html

composer require psr/container
来源：http://hz.cqqwz.cn/gtsviekdqj.html

[U76] PHP：简单路由
来源：http://hz.yueranfly.top/gtwtkfajzi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtiheqslhl.html

[U77] PHP：模板渲染
来源：http://hz.zdqjudy.top/gtpucnxkso.html

composer require twig/twig
来源：http://hz.yongpay.top/gtutswchgi.html

[U78] PHP：单元测试
来源：http://hz.fengsongda.top/gtktdkexyj.html

composer require --dev phpunit/phpunit
来源：http://hz.xziqi.cn/gtqzqpvihd.html

[U79] PHP：静态分析
来源：http://hz.daxiang520.top/gtafwjuzas.html

composer require --dev phpstan/phpstan
来源：http://hz.guowangkeji.top/gtsdrigqza.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtfyyifeqx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhaomingkeji.xyz/gtasbwqpbi.html

[U81] JS：初始化项目
来源：http://hz.ydzc1.top/gttprmpunl.html

npm init -y;  npm i express
来源：http://hz.jyoumei.cn/gtagiphbpe.html

[U82] JS：package.json 脚本
来源：http://hz.yangfankeji.com/gtzqvcqmmv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tian-w.cn/gtlojpfvlg.html

[U83] JS：ES Module 导入导出
来源：http://hz.ppjwa.cn/gtpdzpwaoa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtfxrasyae.html

[U84] JS：CommonJS 写法
来源：http://hz.yanxiufei.cn/gtzffjjacn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sufxvd.cn/gtxowjrcfm.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gttggcuknl.html

a?.b?.c
来源：http://hz.cashguo.top/gtcqlrrkji.html

[U86] JS：空值合并
来源：http://hz.tian-w.cn/gtvlqyfdrc.html

a ?? b
来源：http://hz.daria6918.cn/gtuvqnlkin.html

[U87] JS：解构默认值
来源：http://hz.tianlin.xyz/gtemonnzvv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jianghu66.top/gtaaeuwiun.html

[U88] JS：对象展开合并
来源：http://hz.zhiwuduotai.top/gtlfxwvupl.html

{ ...a, ...b }
来源：http://hz.zdqjudy.top/gtphowpalj.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtrezajyve.html

[...new Set(arr)]
来源：http://hz.hysaishi.cn/gtkoudsgze.html

[U90] JS：数字数组排序
来源：http://hz.hywenlv.cn/gtqojgkrhd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtzjclihfe.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtzhrbascn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.redwolf501.top/gtiuneireu.html

[U92] JS：深拷贝
来源：http://hz.fzhhl.top/gtqtlssrex.html

structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gttkcixvve.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtynuijhtv.html

`共 ${n} 条`
来源：http://hz.gzhubu.top/gtnicbhqty.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gticgywvqn.html

const double = x => x * 2;
来源：http://hz.shangyingyoupin.top/gtkftirper.html

[U95] JS：Promise 包装
来源：http://hz.fengsongda.top/gtkrikmgyt.html

new Promise((resolve, reject) => {})
来源：http://hz.nwbrower.top/gtncpftusw.html

[U96] JS：async/await 与异常
来源：http://hz.ywan-chungtsiang.top/gtrvkjdlwa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtcjitfhhs.html

[U97] JS：并发请求
来源：http://hz.yanxiufei.cn/gtkvsobcuv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtenzijacl.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhaomingkeji.xyz/gtkshglnef.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.quarkkingdee.top/gtkniahwpd.html

[U99] JS：事件监听
来源：http://hz.gaohongyu789.top/gtnlqelpmg.html

el.addEventListener("click", e => {})
来源：http://hz.aizwys.cn/gtiusdrlcu.html

[U100] JS：DOM 查询
来源：http://hz.hfpthk.cn/gtdgbwbtpe.html

document.querySelector(".item")
来源：http://hz.nanxinkj.top/gtwbrtcejc.html

[U101] JS：classList 操作
来源：http://hz.xuetiantiany.cn/gtiivbolao.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gtmpzajnti.html

[U102] JS：本地存储
来源：http://hz.snrcjt.cn/gtetmbrifl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gogol.net.cn/gtgwdgxdch.html

[U103] JS：定时器
来源：http://hz.guannengcc.top/gtcqrtdhol.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinyuanbaomall.cn/gtgnwkwexy.html

[U104] JS：防抖
来源：http://hz.yanxiufei.cn/gtrgnvhjof.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtecdniqfa.html

[U105] JS：节流
来源：http://hz.iojbl.cn/gtxdoouucb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yongpay.top/gtpvcbywaz.html

[U106] JS：日期格式化
来源：http://hz.yueranfly.top/gtpvebnipr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhengqikj.top/gtjymgtana.html

[U107] JS：数字千分位
来源：http://hz.gaohongyu789.top/gtymtcdmoq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgufenzy.top/gtgdwgawwd.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtwkziegex.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtvrouktyl.html

[U109] JS：数组分组
来源：http://hz.yangfankeji.com/gtfkknemhm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtlbzqccdl.html

[U110] JS：数组分块
来源：http://hz.c1oappe.top/gtmlbpswwm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.feifeiyinyue.top/gtqtjcdspg.html

[U111] JS：对象转 Map
来源：http://hz.nanxuanxn.top/gtouxgurew.html

new Map(Object.entries(obj))
来源：http://hz.zhixingplan.top/gtdofcfspx.html

[U112] JS：字符串补位
来源：http://hz.yvedp.cn/gtujegizrb.html

"7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtnarzifta.html

[U113] JS：正则替换全部
来源：http://hz.yueranfly.top/gtyerohzlo.html

s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtydgsmmuz.html

[U114] JS：JSON 深比较
来源：http://hz.nanxuanxn.top/gtoxspiywl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtldunbnmt.html

[U115] JS：生成 UUID
来源：http://hz.sxryk.cn/gtpoywspoe.html

crypto.randomUUID()
来源：http://hz.yuxming.cn/gtqxnyvvla.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.bjfxy.top/gtpjcdqptg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuanzhike.top/gtzppfgxwo.html

[U117] JS：单元测试
来源：http://hz.redwolf501.top/gtdftgssvo.html

npm i -D vitest;  npx vitest
来源：http://hz.c1oappe.top/gtecospcfz.html

[U118] JS：开发服务器
来源：http://hz.aibaodan.cn/gtznvfptor.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gtfvrvrnyl.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtxpsrqsjy.html

npx vite build
来源：http://hz.yj202588.top/gtuxegiqki.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.feifeiyinyue.top/gtsnqahnye.html

import.meta.env.VITE_API_URL
来源：http://hz.gzhubu.top/gtamvtxipr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmkoiukei.html

统计汇总
来源：http://hz.sweek.top/gtrdcdahks.html

================================================================================
来源：http://hz.yvedp.cn/gtenoriiwx.html

按语言统计（条）：
来源：http://hz.cucudq.cn/gtmtwiafuu.html

Python ......... 252
来源：http://hz.kuanghao11.cn/gtffbvbjir.html

PHP ............ 252
来源：http://hz.nanxuanxn.top/gteipcpxwh.html

JavaScript ..... 252
来源：http://hz.sysykeji.top/gtrmscdevo.html

TypeScript ..... 212
来源：http://hz.meibo888.top/gtjzrtotbq.html

Java ........... 212
来源：http://hz.jyoumei.cn/gtlmttxnvs.html

Go ............. 212
来源：http://hz.yuanzhike.top/gtlhgpprkk.html

Ruby ........... 212
来源：http://hz.nanxinkj.top/gtxraygkvm.html

C# ............. 212
来源：http://hz.havefunace.top/gtbkvakiis.html

C .............. 30
来源：http://hz.chenjidiqi.icu/gtbegwcpfx.html

C++ ............ 30
来源：http://hz.ehwqpu.com/gtzktthnqa.html

SQL ............ 90
来源：http://hz.sweek.top/gtyigqfogn.html

Bash ........... 80
来源：http://hz.wangdashe.top/gtwxoefgcd.html

Kotlin ......... 15
来源：http://hz.iojbl.cn/gtkmftdpwr.html

Swift .......... 15
来源：http://hz.tanke756.top/gtnjjnmgtv.html

Lua ............ 10
来源：http://hz.daxiang520.top/gtgsyhszhk.html

Perl ........... 10
来源：http://hz.hammf.cn/gtgqrsggss.html

Scala .......... 10
来源：http://hz.ybcxt.top/gtoyytzugq.html

------------------------------------
来源：http://hz.ybcxt.top/gtfujspgba.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtctpyciis.html

按章节统计：
来源：http://hz.nanxuanxn.top/gtrltzbopo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yuxming.cn/gtcyelsmon.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gthwpsmcgi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gttrcvyupd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gtyjoeybwo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sweek.top/gtsiqkopkr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtclucnzjv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtqvuzxjmz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtuqbllrpg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gteuxefhfm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinqigufen.top/gtwefbvogn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtlreinnxo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gttoescqoj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtzmorjztx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ppjwa.cn/gtnfltxmcz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hnxiangtu.top/gtpuzwxtkn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtpidihuvr.html

Q SQL 专题                              90
来源：http://hz.meibo888.top/gtroopmxlb.html

R Bash 专题                             80
来源：http://hz.jlsjyb.cn/gtbkulppem.html

S C / C++ 专题                          60
来源：http://hz.yangfankeji.com/gttawdkihr.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gtfezyevkx.html

U 高频实用片段                         120
来源：http://hz.yonumen.top/gtjvscxvxy.html

------------------------------------
来源：http://hz.yj20258888.top/gtbhkwkxuu.html

合计                                  2106 条
来源：http://hz.xingfuxueyuan.xyz/gtfgzsgbvr.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtyfyjtrzj.html

使用提醒
来源：http://hz.zdqjudy.top/gtoanayqsl.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gteeymptmy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dashuyun.cn/gttkenrbdn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtjfaifvya.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shzxlz.cn/gtlrupxrcj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cqqwz.cn/gtbzpntgtv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cdnleiting.top/gtfkwtwszr.html

—— 文件结束 ——
来源：http://hz.gzhubu.top/gtnnfkspws.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsermeaue.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yj20258888.top/gtzmhbvjba.html

Common Programming Examples Cheat Book
来源：http://hz.sysykeji.top/gtywgdfscs.html

================================================================================
来源：http://hz.zdqjudy.top/gtvatgywdn.html

【收录内容】
来源：http://hz.yj20258.top/gtxwjitxzy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xziqi.cn/gtibuuvrrh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtkuezjmxa.html

SQL · Bash · C · C++
来源：http://hz.iojbl.cn/gtajbvcpdu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jlsjyb.cn/gtxfmkbflk.html

【使用说明】
来源：http://hz.xuanzx.com/gtbeblhmta.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.andypj.xyz/gtqjravsgh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cheryme.top/gtbwmmbtzh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cdnleiting.top/gtoxdudgeh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cucudq.cn/gthxyjawpk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhaomingkeji.xyz/gtulubkukf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sxryk.cn/gtzfwpdjhg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.meibo888.top/gtvkutetlm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.bjfxy.top/gtmrzivpeo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.aibaodan.cn/gtvknvfczx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.52xcode.cn/gtvroxmjiu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ppjwa.cn/gtkpnbdkdp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.meibo888.top/gtapcnakmy.html

【文件统计】
来源：http://hz.ydzc1.top/gtobldylqg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhixingplan.top/gtznoiysij.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gttivsbthr.html

目  录
来源：http://hz.ivvv.top/gtpkcinzmp.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtzgygmmok.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenlongwang.top/gtqxxpiqjy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtcsihbvks.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtnhhamhcr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtatrwpqzv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xuanzx.com/gtdulusyzk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yangfankeji.com/gtkkrhxziy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aibaodan.cn/gtxzythlul.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.fengsongda.top/gtknvyjnqh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtxjgammsx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gzhubu.top/gtzqotctni.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtkhnchbzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtddwcjfzf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gticpsbwza.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ehwqpu.com/gtnvcdqtys.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xuanzx.com/gtiuhuttun.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtasmvpdip.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.iojbl.cn/gtrswbegub.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.wangshuangyany.cn/gtzfdoibyp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhixingplan.top/gttkwcophv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtlviozmsg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtjfknbtlf.html

================================================================================
来源：http://hz.meibo888.top/gtbrrmquhv.html

A. 基础语法与类型
来源：http://hz.chenlongwang.top/gtxzkgaili.html

================================================================================
来源：http://hz.ppjwa.cn/gtzejpgdlc.html

[A01] Hello World
来源：http://hz.tian-w.cn/gtxlmylaih.html

Py:   print("Hello, World!")
来源：http://hz.zhiwuduotai.top/gtsbolzvtf.html

PHP:  echo "Hello, World!";
来源：http://hz.cheryme.top/gtufjloiyd.html

JS:   console.log("Hello, World!");
来源：http://hz.kuanghao11.cn/gthiztamvo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258.top/gtftgrxgye.html

Java: System.out.println("Hello, World!");
来源：http://hz.yangfankeji.com/gtbgmsvsit.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtyqijihrs.html

Ruby: puts "Hello, World!"
来源：http://hz.meibo888.top/gtpjpufrjm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhoulong.xyz/gtzpiugife.html

[A02] 变量声明与赋值
来源：http://hz.ywan-chungtsiang.top/gtswcroksu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuetiantiany.cn/gtkpesednz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yongpay.top/gtzpukrpvn.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.316326.xyz/gtjplocvej.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.shuidangran.top/gtdhyfyonw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gotoacloud.top/gtnmtadhqn.html

Go:   name := "Alex"; age := 20
来源：http://hz.ivvv.top/gtiaxlamvr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jiagoushi.top/gtxjbltjsw.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtahqpdufu.html

[A03] 常量定义
来源：http://hz.pengpengdd.cyou/gttotzmgac.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.cqqwz.cn/gtsaoxxdqt.html

PHP:  const PI = 3.14159;
来源：http://hz.jiagoushi.top/gtichhnmui.html

JS:   const PI = 3.14159;
来源：http://hz.fengsongda.top/gtvfmibtqm.html

TS:   const PI: number = 3.14159;
来源：http://hz.jinqigfzy.top/gtotrxrckk.html

Java: static final double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtjvndqrku.html

Go:   const PI = 3.14159
来源：http://hz.cheryme.top/gtxaifndmc.html

Ruby: PI = 3.14159
来源：http://hz.zhijiandao.cn/gtoxdzscpy.html

C#:   const double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtupbeylew.html

[A04] 判断变量类型
来源：http://hz.cheryme.top/gtsaglyauq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gtxtucdeji.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gogol.net.cn/gtegufjfnx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tianlin.xyz/gtuygmdjiz.html

TS:   typeof x; x instanceof Date
来源：http://hz.guowangkeji.top/gtpoqafpxw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jiagoushi.top/gtscwkolyr.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shuidangran.top/gtbjqbmffx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.daxiang520.top/gthdbcbeex.html

C#:   x.GetType().Name; x is int
来源：http://hz.jiagoushi.top/gtfivcwvoi.html

[A05] 整数除法与取模
来源：http://hz.gogol.net.cn/gtmrbneake.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ehwqpu.com/gtfdcpylim.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hnqzz.top/gtotbzhlxb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgufenzy.top/gtqwtvkmch.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cashguo.top/gtjjlyelps.html

Java: 7 / 2; 7 % 2
来源：http://hz.sweek.top/gtadchcxfj.html

Go:   7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtvkcftvyx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtsqivufhi.html

C#:   7 / 2; 7 % 2
来源：http://hz.sxryk.cn/gtxfshctjy.html

[A06] 字符串转数字
来源：http://hz.316326.xyz/gtxhybiiuu.html

Py:   int("42"); float("3.14")
来源：http://hz.zdqjudy.top/gtckmlcyrh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shanyushiyangtech.top/gtveklbicl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aizwys.cn/gteeywfjvw.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.haohaochexian.top/gtxjcebcaz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenjidiqi.icu/gtvvvgymgx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xuanzx.com/gthhxpjznr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gogol.net.cn/gtktipneba.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.cqqwz.cn/gtwpvxxsao.html

[A07] 数字转字符串
来源：http://hz.shzxlz.cn/gteqhqypin.html

Py:   str(42)
来源：http://hz.andypj.xyz/gtxxfommmi.html

PHP:  (string) 42; strval(42)
来源：http://hz.shanyushiyangkeji.top/gthpiaaoeq.html

JS:   String(42); (42).toString()
来源：http://hz.ydzc1.top/gtsoazoywo.html

TS:   String(42)
来源：http://hz.guowangkeji.top/gtxwozaukx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hywenlv.cn/gtqoazbqdp.html

Go:   strconv.Itoa(42)
来源：http://hz.sysykeji.top/gtoapxtqun.html

Ruby: 42.to_s
来源：http://hz.snrcjt.cn/gtxyexsxto.html

C#:   42.ToString()
来源：http://hz.nanxinkj.top/gtuqxxlnnn.html

[A08] 取整与四舍五入
来源：http://hz.zdqjudy.top/gtyjvqvuho.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.snrcjt.cn/gtlmapfvvi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dashuyun.cn/gtyphpugkt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.dashuyun.cn/gtjilwagkn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.smart0.xyz/gtpomexfcb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtosbgbuvf.html


<!-- 参考信息 -->