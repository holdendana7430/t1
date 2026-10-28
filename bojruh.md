代发 wailian999

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gthafhzebv.html

public readonly string $name
来源：http://hz.daxiang520.top/gtfgdyrzmu.html

[U50] PHP：构造器属性提升
来源：http://hz.shanyushiyangtech.top/gtfewswgpz.html

public function __construct(private int $id) {}
来源：http://hz.hnqzz.top/gtblvpfmuv.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtujwzlxcg.html

[$a, $b] = $arr;
来源：http://hz.xziqi.cn/gtwhogtxxh.html

[U52] PHP：箭头函数
来源：http://hz.dashuyun.cn/gtmtdzhafj.html

$double = fn($x) => $x * 2;
来源：http://hz.redwolf501.top/gtehtrvrtv.html

[U53] PHP：空合并运算符
来源：http://hz.yongpay.top/gtcrszgufq.html

$v = $a ?? $b ?? "default";
来源：http://hz.bjfxy.top/gtcikrobjd.html

[U54] PHP：空安全调用
来源：http://hz.dashuyun.cn/gtpmqjjwnm.html

$obj?->method()
来源：http://hz.nwbrower.top/gtsckpzmol.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtvjtxyydk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.daxiang520.top/gtlkqmuokl.html

[U56] PHP：命名参数
来源：http://hz.iojbl.cn/gtztnywjek.html

f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtilrzxicd.html

[U57] PHP：字符串插值
来源：http://hz.zycfv.cn/gtaslwckex.html

"值: {$a}"
来源：http://hz.mhx1999.top/gtncreuqyn.html

[U58] PHP：数组三件套
来源：http://hz.gaohongyu789.top/gtztmixual.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtnwuzqozd.html

[U59] PHP：自定义排序
来源：http://hz.kuanghao11.cn/gtefflpegr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtygflolfv.html

[U60] PHP：JSON 编解码
来源：http://hz.pengpengdd.cyou/gtauuwuyrk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhaomingkeji.xyz/gtywgokdvx.html

[U61] PHP：正则
来源：http://hz.shanyushiyangkeji.top/gtxtdzohda.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtprmbzasu.html

[U62] PHP：日期对象
来源：http://hz.guannengcc.top/gtxqqgfrcm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tanke756.top/gtkhtwgywi.html

[U63] PHP：文件读写
来源：http://hz.yongpay.top/gtlptxnflw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtidjzclrr.html

[U64] PHP：目录遍历
来源：http://hz.yvedp.cn/gtnqjtarru.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.pycfn.com/gtfntctvsb.html

[U65] PHP：会话
来源：http://hz.haohaochexian.top/gtgmznkjis.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.daxiang520.top/gtjbyocfzz.html

[U66] PHP：设置 Cookie
来源：http://hz.vqdsnc.cn/gtvvpqdtbk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sweek.top/gtwofrzvnz.html

[U67] PHP：处理文件上传
来源：http://hz.yueranfly.top/gthaalmcbm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.haohaochexian.top/gthsjjuhod.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangtech.top/gtnrdcoowa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sufxvd.cn/gtkkfadtlw.html

[U69] PHP：PDO 预处理
来源：http://hz.hongshengwenyu.top/gtpchkcvkl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shangyingyoupin.top/gtkhslefzy.html

[U70] PHP：PDO 事务
来源：http://hz.pengpengdd.cyou/gtvbrgqzgk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhoulong.xyz/gtaqiglklo.html

[U71] PHP：抛出异常
来源：http://hz.quarkkingdee.top/gtqnwivtfq.html

throw new RuntimeException("失败", 500);
来源：http://hz.dianchejie.cn/gtjerjqkrb.html

[U72] PHP：写错误日志
来源：http://hz.52xcode.cn/gtsvuonbpk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gzhubu.top/gtptzvfshm.html

[U73] PHP：读取 ini 配置
来源：http://hz.gaohongyu789.top/gteahxsvzg.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gthnemcwbx.html

[U74] PHP：读取环境变量
来源：http://hz.nwbrower.top/gttnjglefa.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtzukhftql.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gtmowvanjf.html

composer require psr/container
来源：http://hz.cdnleiting.top/gtrdvaauen.html

[U76] PHP：简单路由
来源：http://hz.cqqwz.cn/gtfuqvkeep.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhixingplan.top/gtymaewdka.html

[U77] PHP：模板渲染
来源：http://hz.xylfe.cn/gtngjffzuk.html

composer require twig/twig
来源：http://hz.xuanzx.com/gtotswdkdy.html

[U78] PHP：单元测试
来源：http://hz.hongshengwenyu.top/gtxhcuzzmb.html

composer require --dev phpunit/phpunit
来源：http://hz.yuxming.cn/gtfqwcmpmx.html

[U79] PHP：静态分析
来源：http://hz.vqdsnc.cn/gtsxorshep.html

composer require --dev phpstan/phpstan
来源：http://hz.jinyuanbaomall.cn/gtkxaxwxgj.html

[U80] PHP：代码规范修复
来源：http://hz.nwbrower.top/gtxtduzlye.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.vqdsnc.cn/gtfqeiatdc.html

[U81] JS：初始化项目
来源：http://hz.sufxvd.cn/gtgbtgynzy.html

npm init -y;  npm i express
来源：http://hz.smart0.xyz/gtyqncazsq.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtrxdxsbzk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtvsnutdsg.html

[U83] JS：ES Module 导入导出
来源：http://hz.smart0.xyz/gtnacuzcku.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.redwolf501.top/gtworeqbaj.html

[U84] JS：CommonJS 写法
来源：http://hz.ehwqpu.com/gtjtclgufe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pycfn.com/gthraoyaoq.html

[U85] JS：可选链
来源：http://hz.hfpthk.cn/gtzgoiqnfx.html

a?.b?.c
来源：http://hz.yj202588.top/gthsmpkalc.html

[U86] JS：空值合并
来源：http://hz.ppjwa.cn/gtxghcxawg.html

a ?? b
来源：http://hz.snrcjt.cn/gtyxnwvhex.html

[U87] JS：解构默认值
来源：http://hz.zhiwuduotai.top/gtubsukzoc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinghuilouyu.cn/gttvyhcrqg.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtwnrcbusx.html

{ ...a, ...b }
来源：http://hz.zhaomingkeji.xyz/gtyhfznqqd.html

[U89] JS：数组去重
来源：http://hz.ybcxt.top/gtlrsszyfl.html

[...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtbeuunury.html

[U90] JS：数字数组排序
来源：http://hz.snrcjt.cn/gtgrggtkjw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtkmivvoht.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtogpyxxuu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ybcxt.top/gtipcesckw.html

[U92] JS：深拷贝
来源：http://hz.jinghuilouyu.cn/gtjreiffoa.html

structuredClone(obj)
来源：http://hz.cheryme.top/gtrmsakaxv.html

[U93] JS：模板字符串
来源：http://hz.52xcode.cn/gtjllnukmo.html

`共 ${n} 条`
来源：http://hz.svipenyu.cn/gtfvvwbiux.html

[U94] JS：箭头函数
来源：http://hz.zhixingplan.top/gtnzxihqet.html

const double = x => x * 2;
来源：http://hz.cucudq.cn/gtcgooqifd.html

[U95] JS：Promise 包装
来源：http://hz.chenlongwang.top/gtqjfelncc.html

new Promise((resolve, reject) => {})
来源：http://hz.vqdsnc.cn/gtujbflplc.html

[U96] JS：async/await 与异常
来源：http://hz.yueranfly.top/gtuhlvoeoh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtiozhofzq.html

[U97] JS：并发请求
来源：http://hz.sufxvd.cn/gtqfjcwhvz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtgvlxisvx.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj202588.top/gtassxjezd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenjidiqi.icu/gtnzparquo.html

[U99] JS：事件监听
来源：http://hz.cucudq.cn/gtbzbjucfw.html

el.addEventListener("click", e => {})
来源：http://hz.birdmap.top/gtwxdcyfrm.html

[U100] JS：DOM 查询
来源：http://hz.yuxming.cn/gtzrgmkwyo.html

document.querySelector(".item")
来源：http://hz.cucudq.cn/gtbeurttwy.html

[U101] JS：classList 操作
来源：http://hz.jyoumei.cn/gtvykincyv.html

el.classList.toggle("active")
来源：http://hz.dianchejie.cn/gtxzrakgeo.html

[U102] JS：本地存储
来源：http://hz.shangyingyoupin.top/gtayqmikli.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnqzz.top/gtbgqnceqt.html

[U103] JS：定时器
来源：http://hz.bjfxy.top/gtuiycyhnb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aibaodan.cn/gtvazmdhjk.html

[U104] JS：防抖
来源：http://hz.hammf.cn/gtmbdrspdj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtffknymyp.html

[U105] JS：节流
来源：http://hz.xinyue.icu/gtwvyxshsp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shuidangran.top/gtloivdvpm.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gtyxfttxzx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xuanzx.com/gtbvijhpjj.html

[U107] JS：数字千分位
来源：http://hz.hywenlv.cn/gtjvxxzrtu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dashuyun.cn/gtrllqesob.html

[U108] JS：随机整数
来源：http://hz.zhiwuduotai.top/gttumprtii.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.dianchejie.cn/gtzqmwacun.html

[U109] JS：数组分组
来源：http://hz.daxiang520.top/gtvzzhuxgm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtudkaawrg.html

[U110] JS：数组分块
来源：http://hz.fengsongda.top/gtfgadfpvn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gzhubu.top/gtvobpuwzt.html

[U111] JS：对象转 Map
来源：http://hz.yuxming.cn/gteqrspynj.html

new Map(Object.entries(obj))
来源：http://hz.yuxming.cn/gtiuckryht.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtzsberslb.html

"7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtfwncsatr.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gtiixdlxxa.html

s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtknpvfrwo.html

[U114] JS：JSON 深比较
来源：http://hz.snrcjt.cn/gtshtixtwf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gttgpizfsf.html

[U115] JS：生成 UUID
来源：http://hz.yonumen.top/gtfjvfueoy.html

crypto.randomUUID()
来源：http://hz.c1oappe.top/gthccchtyn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ivvv.top/gthiuhqimo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhengqikj.top/gthydndezh.html

[U117] JS：单元测试
来源：http://hz.shzxlz.cn/gtnqhbnkiq.html

npm i -D vitest;  npx vitest
来源：http://hz.ppjwa.cn/gtwvlbtnla.html

[U118] JS：开发服务器
来源：http://hz.redwolf501.top/gtynntvabi.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gtmallzjeg.html

[U119] JS：生产构建
来源：http://hz.jinghuilouyu.cn/gtczpyxhfr.html

npx vite build
来源：http://hz.yueranfly.top/gtlwagwvfq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhixingplan.top/gtnyydlnld.html

import.meta.env.VITE_API_URL
来源：http://hz.chenlongwang.top/gtmvcjsoda.html

================================================================================
来源：http://hz.yuanzhike.top/gtfiifbyin.html

统计汇总
来源：http://hz.xinyue.icu/gtmcersmtx.html

================================================================================
来源：http://hz.wangdashe.top/gtyuitbsoa.html

按语言统计（条）：
来源：http://hz.zycfv.cn/gtwrhgqncw.html

Python ......... 252
来源：http://hz.wangshuangyany.cn/gtfhnzmsmf.html

PHP ............ 252
来源：http://hz.nanxuanxn.top/gtkhojrnuu.html

JavaScript ..... 252
来源：http://hz.hammf.cn/gtoigvcssf.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gtuqbrbjhw.html

Java ........... 212
来源：http://hz.hysaishi.cn/gtzurogrli.html

Go ............. 212
来源：http://hz.ywan-chungtsiang.top/gtrbynhken.html

Ruby ........... 212
来源：http://hz.hnxiangtu.top/gtzoznjlbb.html

C# ............. 212
来源：http://hz.yongpay.top/gtcvwohgjk.html

C .............. 30
来源：http://hz.daxiang520.top/gtnhliwwxh.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtapbyfyfm.html

SQL ............ 90
来源：http://hz.birdmap.top/gtduppasbs.html

Bash ........... 80
来源：http://hz.nwbrower.top/gtkguaiyvr.html

Kotlin ......... 15
来源：http://hz.ydzc1.top/gtckadhidb.html

Swift .......... 15
来源：http://hz.sysykeji.top/gtjijbvjrb.html

Lua ............ 10
来源：http://hz.52xcode.cn/gtjdygoggi.html

Perl ........... 10
来源：http://hz.hfpthk.cn/gtxlvnrysb.html

Scala .......... 10
来源：http://hz.yangfankeji.com/gtovftjdrs.html

------------------------------------
来源：http://hz.fzhhl.top/gtbyvimntj.html

合计 ........... 2106 条
来源：http://hz.shangyingyoupin.top/gtonewgcrm.html

按章节统计：
来源：http://hz.ydjk.org.cn/gtwcrprdnf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtxjbjkoyl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.havefunace.top/gtsxesyzdz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtsxwjazpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtefqtsikv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fzhhl.top/gttksfvoyj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtpcuxvqxt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtskqtvmlv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtbdumbgsz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtjpfsvlxi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtboxmtmcc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtqycqhdyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtyvgneayy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtbzctndsf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xziqi.cn/gthhywbome.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ydjk.org.cn/gtdfkdrnfe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yanxiufei.cn/gtriufsijq.html

Q SQL 专题                              90
来源：http://hz.nanxuanxn.top/gtydvvmdck.html

R Bash 专题                             80
来源：http://hz.52xcode.cn/gtkkdxbjbr.html

S C / C++ 专题                          60
来源：http://hz.pengpengdd.cyou/gtazmqshze.html

T 其他语言补充                          60
来源：http://hz.shangyingyoupin.top/gtswxcabzs.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtqtisyfch.html

------------------------------------
来源：http://hz.yangfankeji.com/gtvyrcxfcm.html

合计                                  2106 条
来源：http://hz.guannengcc.top/gtclakvsxd.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtchgtbbmi.html

使用提醒
来源：http://hz.hnqzz.top/gtvkzsunjf.html

--------------------------------------------------------------------------------
来源：http://hz.hnqzz.top/gtwvvazzno.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hywenlv.cn/gtlqqxvrnf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cdnleiting.top/gtfolicsuy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cucudq.cn/gtzdmzglxq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hongshengwenyu.top/gtojceddwg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yueranfly.top/gtqopkskvj.html

—— 文件结束 ——
来源：http://hz.sweek.top/gtahdsodbk.html

================================================================================
来源：http://hz.zycfv.cn/gtklaeyubs.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aibaodan.cn/gtzoocsgqf.html

Common Programming Examples Cheat Book
来源：http://hz.xylfe.cn/gtswqplfnh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtomzvyjph.html

【收录内容】
来源：http://hz.redwolf501.top/gtryieqkfb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yanxiufei.cn/gtbakdukxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.sweek.top/gtivzjuiys.html

SQL · Bash · C · C++
来源：http://hz.hammf.cn/gtpdjslebt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtttwfehoa.html

【使用说明】
来源：http://hz.pycfn.com/gtpcqjzmby.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nanxuanxn.top/gtwyaqgbwt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cheryme.top/gtinlidxiu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gteomduegp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.andypj.xyz/gtpecneaug.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sweek.top/gtxmstdgua.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.0kj1m.cn/gtmkqwxavj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenlongwang.top/gtpnsodper.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.feifeiyinyue.top/gtndbgrypn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.wangshuangyany.cn/gtlomtqhvv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jlsjyb.cn/gtgpcdgiez.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.c1oappe.top/gtmxeueryl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hfpthk.cn/gtesjodmky.html

【文件统计】
来源：http://hz.xuetiantiany.cn/gtlpeewelj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.feifeiyinyue.top/gtapcoygtd.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtdugrmava.html

目  录
来源：http://hz.sxryk.cn/gtfzlxhbcf.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtakowrumb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtoxznyubo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhoulong.xyz/gtwqfsgnjo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtexgarmax.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtpwkkffvk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hnxiangtu.top/gtezgxlcue.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.sxryk.cn/gtazxjrykg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtarnsokog.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtrkfqqbpg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtvtgtfvgc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj202588.top/gtymhbwqin.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtaxdrowsa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtskkwlrpe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtklhujyei.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtknrrwulh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nanxuanxn.top/gtxjsjmifo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtvllksocl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.bjfxy.top/gtqcpkyrya.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhengqikj.top/gtvqsehfxn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shzxlz.cn/gtbrdhxypc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtzjfswajc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.smart0.xyz/gtzgdammhy.html

================================================================================
来源：http://hz.xinyue.icu/gtzxomopue.html

A. 基础语法与类型
来源：http://hz.fengsongda.top/gtczrgcrnh.html

================================================================================
来源：http://hz.yj20258.top/gtjprnljxu.html

[A01] Hello World
来源：http://hz.snrcjt.cn/gttsqwyipe.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtbqfjruvj.html

PHP:  echo "Hello, World!";
来源：http://hz.yanxiufei.cn/gtjcogdgqh.html

JS:   console.log("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtmyqeyfxv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yvedp.cn/gtnqpcfwzn.html

Java: System.out.println("Hello, World!");
来源：http://hz.shzxlz.cn/gtuuzcllyx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.haohaochexian.top/gtfzufmidz.html

Ruby: puts "Hello, World!"
来源：http://hz.316326.xyz/gtgatpzlld.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tanke756.top/gtgdwkkvdu.html

[A02] 变量声明与赋值
来源：http://hz.cdnleiting.top/gtqxezslco.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zycfv.cn/gtrtqhguic.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fzhhl.top/gtitcdwocx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shangyingyoupin.top/gtphfcvxcm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.iojbl.cn/gtisnyudfz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtzyfbbcbs.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhoulong.xyz/gtsyfxzive.html

Ruby: name = "Alex"; age = 20
来源：http://hz.wangdashe.top/gttfgffjqa.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.9152youxi.cn/gtqysmfyzy.html

[A03] 常量定义
来源：http://hz.tianlin.xyz/gtousbyuaj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.dashuyun.cn/gtqqphcuxd.html

PHP:  const PI = 3.14159;
来源：http://hz.yueranfly.top/gtdnovhiqu.html

JS:   const PI = 3.14159;
来源：http://hz.fzhhl.top/gtcqsysgct.html

TS:   const PI: number = 3.14159;
来源：http://hz.xylfe.cn/gtmnrmbcdj.html

Java: static final double PI = 3.14159;
来源：http://hz.daria6918.cn/gtdpsmdnyv.html

Go:   const PI = 3.14159
来源：http://hz.yj20258888.top/gtirpwfkqw.html

Ruby: PI = 3.14159
来源：http://hz.iojbl.cn/gtmpsrsimg.html

C#:   const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtzjmzlvxa.html

[A04] 判断变量类型
来源：http://hz.chenjidiqi.icu/gtfxuuuzop.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yuxming.cn/gtkcnpxacv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hnxiangtu.top/gtipmpkjiq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xinyue.icu/gthdcxwfny.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj20258.top/gtyxdpntov.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.mhx1999.top/gtcjjmrgzx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuanzhike.top/gtmtfaiwmp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shuidangran.top/gtcerxkoiq.html

C#:   x.GetType().Name; x is int
来源：http://hz.cashguo.top/gtlkwfgsxy.html

[A05] 整数除法与取模
来源：http://hz.hysaishi.cn/gtmizoocxi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yongpay.top/gtaphrtnun.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhiwuduotai.top/gtbyckmflu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yvedp.cn/gtezsegotg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yvedp.cn/gtfoqhcrvi.html

Java: 7 / 2; 7 % 2
来源：http://hz.iojbl.cn/gtwgnaatmv.html

Go:   7 / 2; 7 % 2
来源：http://hz.wangdashe.top/gtfhigdhrw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtmtplwiua.html

C#:   7 / 2; 7 % 2
来源：http://hz.sufxvd.cn/gtakunpfjs.html

[A06] 字符串转数字
来源：http://hz.xziqi.cn/gtwqxbgfdr.html

Py:   int("42"); float("3.14")
来源：http://hz.wangdashe.top/gtiodekqmw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jiagoushi.top/gtozqjfcma.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.nwbrower.top/gttisapxhf.html


<!-- 参考信息 -->