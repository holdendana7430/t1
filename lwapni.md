代发 wailian999

[U47] PHP：联合类型
来源：http://hz.wangdashe.top/gtxxrlfrun.html

int|string $id
来源：http://hz.ivvv.top/gtoxnuhdge.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtnzpbbvot.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gtbrmlopec.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtlsquvtzk.html

public readonly string $name
来源：http://hz.cqqwz.cn/gtcdybbvay.html

[U50] PHP：构造器属性提升
来源：http://hz.yj202588.top/gtdjxoayie.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtrnukdvyr.html

[U51] PHP：数组解构
来源：http://hz.jqgfzy.top/gtvuqcycom.html

[$a, $b] = $arr;
来源：http://hz.yuanzhike.top/gtssgjtkod.html

[U52] PHP：箭头函数
来源：http://hz.fzhhl.top/gtthubkrsa.html

$double = fn($x) => $x * 2;
来源：http://hz.ydzc1.top/gtfjtcojyk.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gtprtbkglf.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydjk.org.cn/gtqmnhghmc.html

[U54] PHP：空安全调用
来源：http://hz.dianchejie.cn/gtmoorbtkx.html

$obj?->method()
来源：http://hz.zycfv.cn/gtadmdjaza.html

[U55] PHP：match 表达式
来源：http://hz.tianlin.xyz/gthhxdzjan.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.316326.xyz/gtahtffscv.html

[U56] PHP：命名参数
来源：http://hz.xylfe.cn/gttdelslhk.html

f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtjvcsnyau.html

[U57] PHP：字符串插值
来源：http://hz.redwolf501.top/gtrareliov.html

"值: {$a}"
来源：http://hz.jinghuilouyu.cn/gtaedqrpfi.html

[U58] PHP：数组三件套
来源：http://hz.zhongyouzk.top/gtvzwtxmdu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhiwuduotai.top/gtlnlkyrxe.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtzchvexon.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtrktikkqs.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangkeji.top/gtpetbdlbz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shzxlz.cn/gtxyflnezj.html

[U61] PHP：正则
来源：http://hz.ivvv.top/gtfhfaxhyv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenlongwang.top/gtvasvirhm.html

[U62] PHP：日期对象
来源：http://hz.jlsjyb.cn/gtxewzjjcb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.havefunace.top/gtzuaabtec.html

[U63] PHP：文件读写
来源：http://hz.yj202588.top/gtaostxqhp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ehwqpu.com/gtqcangddd.html

[U64] PHP：目录遍历
来源：http://hz.smart0.xyz/gtcrhgbobo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj20258888.top/gtcrsitafz.html

[U65] PHP：会话
来源：http://hz.yj202588.top/gttiqaqtld.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtawsmpzjl.html

[U66] PHP：设置 Cookie
来源：http://hz.havefunace.top/gthjmlfhgx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yueranfly.top/gtafjaaodn.html

[U67] PHP：处理文件上传
来源：http://hz.shzxlz.cn/gtnuqxzkdj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aibaodan.cn/gtjlapbfip.html

[U68] PHP：PDO 连接
来源：http://hz.sxryk.cn/gttqtkfrlf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtbssfoout.html

[U69] PHP：PDO 预处理
来源：http://hz.guannengcc.top/gtgbhtsszx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cheryme.top/gtqukfhylf.html

[U70] PHP：PDO 事务
来源：http://hz.zycfv.cn/gtdriaehco.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gtmjpxloce.html

[U71] PHP：抛出异常
来源：http://hz.shzxlz.cn/gtsfpxupuv.html

throw new RuntimeException("失败", 500);
来源：http://hz.feifeiyinyue.top/gtofjjxbvx.html

[U72] PHP：写错误日志
来源：http://hz.hywenlv.cn/gtyjwapdep.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shangyingyoupin.top/gtsleonkjy.html

[U73] PHP：读取 ini 配置
来源：http://hz.9152youxi.cn/gtnmprpzjg.html

parse_ini_file("config.ini", true)
来源：http://hz.ybcxt.top/gtaxzgusjh.html

[U74] PHP：读取环境变量
来源：http://hz.quarkkingdee.top/gturnwnhzc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tianlin.xyz/gtthyqqano.html

[U75] PHP：依赖注入
来源：http://hz.gzhubu.top/gtshwgrkks.html

composer require psr/container
来源：http://hz.nanxuanxn.top/gtwpbpbfie.html

[U76] PHP：简单路由
来源：http://hz.shzxlz.cn/gthupcpxhp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shzxlz.cn/gtiiizdyqs.html

[U77] PHP：模板渲染
来源：http://hz.sysykeji.top/gtzlsntbon.html

composer require twig/twig
来源：http://hz.cashguo.top/gtscujhylm.html

[U78] PHP：单元测试
来源：http://hz.yuxming.cn/gttbjyuswx.html

composer require --dev phpunit/phpunit
来源：http://hz.smart0.xyz/gthxexrgts.html

[U79] PHP：静态分析
来源：http://hz.xingfuxueyuan.xyz/gtzygfivdw.html

composer require --dev phpstan/phpstan
来源：http://hz.aibaodan.cn/gtqvbigffc.html

[U80] PHP：代码规范修复
来源：http://hz.fzhhl.top/gtyabzuust.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.nanxinkj.top/gtzlegsbyg.html

[U81] JS：初始化项目
来源：http://hz.zhoulong.xyz/gtcboxeega.html

npm init -y;  npm i express
来源：http://hz.hnxiangtu.top/gtfzmfhsxb.html

[U82] JS：package.json 脚本
来源：http://hz.birdmap.top/gtzujwbeyr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.wangdashe.top/gtgeqhflol.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gtatcbvriz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtrbvyucrm.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gtryjsteol.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tanke756.top/gtgymzpbws.html

[U85] JS：可选链
来源：http://hz.shangyingyoupin.top/gtxehggfoe.html

a?.b?.c
来源：http://hz.xinyue.icu/gtcrznfgbs.html

[U86] JS：空值合并
来源：http://hz.ywan-chungtsiang.top/gtucmwmicy.html

a ?? b
来源：http://hz.316326.xyz/gtwiqdmqqu.html

[U87] JS：解构默认值
来源：http://hz.yuanzhike.top/gtclgpnmmr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cqqwz.cn/gtznepkrxo.html

[U88] JS：对象展开合并
来源：http://hz.svipenyu.cn/gtrevwfhjy.html

{ ...a, ...b }
来源：http://hz.zhengqikj.top/gthaqczphx.html

[U89] JS：数组去重
来源：http://hz.cdnleiting.top/gttqlhrark.html

[...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtsbgccgvw.html

[U90] JS：数字数组排序
来源：http://hz.jinqigufen.top/gtpsykjmuo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtzbhwqsdl.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtrwqniesw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tianlin.xyz/gtdtpjxddx.html

[U92] JS：深拷贝
来源：http://hz.pycfn.com/gthqbqbrjc.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtruxxpfcm.html

[U93] JS：模板字符串
来源：http://hz.nanxuanxn.top/gtiotvnqta.html

`共 ${n} 条`
来源：http://hz.hnxiangtu.top/gtetkpekws.html

[U94] JS：箭头函数
来源：http://hz.0kj1m.cn/gttyzbwqbr.html

const double = x => x * 2;
来源：http://hz.0kj1m.cn/gthekcwzxb.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gtmspyjzeb.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gthxpezect.html

[U96] JS：async/await 与异常
来源：http://hz.wangdashe.top/gtmsoqukwh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtvsjsbapw.html

[U97] JS：并发请求
来源：http://hz.cqqwz.cn/gtfkqszhdy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtlnmhisfs.html

[U98] JS：fetch 带 JSON
来源：http://hz.cqqwz.cn/gtgycfzhec.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinghuilouyu.cn/gtngbsllwy.html

[U99] JS：事件监听
来源：http://hz.sweek.top/gtqoupieqz.html

el.addEventListener("click", e => {})
来源：http://hz.yvedp.cn/gtpblzyqpl.html

[U100] JS：DOM 查询
来源：http://hz.hongshengwenyu.top/gtrhlwbqnz.html

document.querySelector(".item")
来源：http://hz.gzhubu.top/gtigwhizxf.html

[U101] JS：classList 操作
来源：http://hz.smart0.xyz/gtutxxtroy.html

el.classList.toggle("active")
来源：http://hz.daxiang520.top/gtjeoutmew.html

[U102] JS：本地存储
来源：http://hz.sysykeji.top/gtkyziwfcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.snrcjt.cn/gttnyqvqtp.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gttnbclufo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.iojbl.cn/gtafvzyegf.html

[U104] JS：防抖
来源：http://hz.jianghu66.top/gthhoqffwv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtysleurkn.html

[U105] JS：节流
来源：http://hz.jinghuilouyu.cn/gtlmpeipyz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangshuangyany.cn/gtxwxjhnaw.html

[U106] JS：日期格式化
来源：http://hz.ehwqpu.com/gtqnnwpzbq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.snrcjt.cn/gttyyfyzim.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtenkhgdiz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shuidangran.top/gtbgyawywm.html

[U108] JS：随机整数
来源：http://hz.jinqigufen.top/gtyxfprkdl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jiagoushi.top/gtoysdpkll.html

[U109] JS：数组分组
来源：http://hz.jiagoushi.top/gtwpkmhnxb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.aibaodan.cn/gtqmrmmsqe.html

[U110] JS：数组分块
来源：http://hz.zhixingplan.top/gtflmnvebz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gtexzveqtb.html

[U111] JS：对象转 Map
来源：http://hz.redwolf501.top/gtqpynoyve.html

new Map(Object.entries(obj))
来源：http://hz.smart0.xyz/gtrxgtbiwt.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtemmjzpsa.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtrsyxxipz.html

[U113] JS：正则替换全部
来源：http://hz.kuanghao11.cn/gtcwkparnk.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtrggxntzw.html

[U114] JS：JSON 深比较
来源：http://hz.yongpay.top/gtxkbnccqc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtjxzaaunc.html

[U115] JS：生成 UUID
来源：http://hz.sweek.top/gtqkzluglp.html

crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtubrfzzwp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenjidiqi.icu/gtaptvfsoz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.andypj.xyz/gtkbklvsue.html

[U117] JS：单元测试
来源：http://hz.cdnleiting.top/gtwhudbjdi.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gteyeffxlt.html

[U118] JS：开发服务器
来源：http://hz.jianghu66.top/gtzheomoeq.html

npm i -D vite;  npx vite
来源：http://hz.hnxiangtu.top/gtibjwbiit.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtsnlosuov.html

npx vite build
来源：http://hz.chenlongwang.top/gtsoqbqrrs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtvvaycmca.html

import.meta.env.VITE_API_URL
来源：http://hz.birdmap.top/gtsqbylzmg.html

================================================================================
来源：http://hz.yuanzhike.top/gtssnnyijs.html

统计汇总
来源：http://hz.zdqjudy.top/gtfuvreamw.html

================================================================================
来源：http://hz.9152youxi.cn/gtysdtauqv.html

按语言统计（条）：
来源：http://hz.iojbl.cn/gtjkoxrtfd.html

Python ......... 252
来源：http://hz.shanyushiyangkeji.top/gthpgdhndv.html

PHP ............ 252
来源：http://hz.zdqjudy.top/gtqowqvmel.html

JavaScript ..... 252
来源：http://hz.hammf.cn/gtcclkdmnp.html

TypeScript ..... 212
来源：http://hz.jiagoushi.top/gtjjchzmyg.html

Java ........... 212
来源：http://hz.aizwys.cn/gthdnokpek.html

Go ............. 212
来源：http://hz.nanxinkj.top/gtchiadxnn.html

Ruby ........... 212
来源：http://hz.cashguo.top/gtnqglebqd.html

C# ............. 212
来源：http://hz.feifeiyinyue.top/gtclgumcyn.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtcmjtyhnr.html

C++ ............ 30
来源：http://hz.jinqigfzy.top/gtbempihru.html

SQL ............ 90
来源：http://hz.haohaochexian.top/gtxmzbttok.html

Bash ........... 80
来源：http://hz.mhx1999.top/gtypixvxsr.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtqihsqvya.html

Swift .......... 15
来源：http://hz.shuidangran.top/gtnwnwiarh.html

Lua ............ 10
来源：http://hz.cashguo.top/gtgxifjnwz.html

Perl ........... 10
来源：http://hz.zhoulong.xyz/gtiwavpufa.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gtbalbrtvw.html

------------------------------------
来源：http://hz.havefunace.top/gtubvmxatz.html

合计 ........... 2106 条
来源：http://hz.fzhhl.top/gtzjvauepp.html

按章节统计：
来源：http://hz.zhijiandao.cn/gttyeutmuy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xingfuxueyuan.xyz/gticcjknah.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtbgvnfjja.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtgdreqjhp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtfcwhbiuc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shangyingyoupin.top/gtyxicyunq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj20258888.top/gtxinvemmp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtzadqpbbn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtfqvwnixt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtzdspxobo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtnwvprcsi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtvbogmemk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtaanglvbj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtstfgcjev.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtgmkdirrv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cucudq.cn/gtmrxgxspu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtcjkvorbp.html

Q SQL 专题                              90
来源：http://hz.vqdsnc.cn/gtuppdjsbx.html

R Bash 专题                             80
来源：http://hz.hnxiangtu.top/gtisvflrff.html

S C / C++ 专题                          60
来源：http://hz.iojbl.cn/gtsrjtbraz.html

T 其他语言补充                          60
来源：http://hz.jinyuanbaomall.cn/gtxaeoxnom.html

U 高频实用片段                         120
来源：http://hz.cqqwz.cn/gtsahkfyoe.html

------------------------------------
来源：http://hz.aibaodan.cn/gtlgfrroni.html

合计                                  2106 条
来源：http://hz.shuidangran.top/gtqhpemyxb.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtdjijanlv.html

使用提醒
来源：http://hz.yj20258888.top/gtiyxmztuq.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtzjfijwlo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtxmupabtd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.mhx1999.top/gtpyovegeh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.chenlongwang.top/gtmxmirwcn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.chenzaomai.com/gtmodvjsbm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhengqikj.top/gtjezaamxh.html

—— 文件结束 ——
来源：http://hz.zycfv.cn/gtcljlyldq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmuxdktpy.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nwbrower.top/gtfwrolpsc.html

Common Programming Examples Cheat Book
来源：http://hz.tianlin.xyz/gtjfgawsjw.html

================================================================================
来源：http://hz.aizwys.cn/gtmovdogta.html

【收录内容】
来源：http://hz.ppjwa.cn/gtvgxvsifm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yanxiufei.cn/gttkbjdoby.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gtpvyiludm.html

SQL · Bash · C · C++
来源：http://hz.yuanzhike.top/gtgdmkwdrl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.hywenlv.cn/gtmchduqyy.html

【使用说明】
来源：http://hz.xuanzx.com/gtofbpnzfi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.iojbl.cn/gtrkdkiqam.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtekidhnuk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gtpxjwjqvx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhixingplan.top/gtieioogti.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.dashuyun.cn/gthgeyyzvz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cqqwz.cn/gtsvojjwoq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shuidangran.top/gtehlandpl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ybcxt.top/gtvrlnvojz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gteurmntax.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.9152youxi.cn/gttjtzokki.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ybcxt.top/gthloqourt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sxryk.cn/gthvrkmfkn.html

【文件统计】
来源：http://hz.c1oappe.top/gtmzscpaek.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ydzc1.top/gtcycbhnfg.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtcndqdsag.html

目  录
来源：http://hz.quarkkingdee.top/gtgwyzreao.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtoklthyjw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nwbrower.top/gtmatflbbs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtvlncocae.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.gaohongyu789.top/gtvuffnand.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtjtosfufn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fengsongda.top/gtcjbxkfep.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gtqrnglryx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.fengsongda.top/gtewqxzotp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhixingplan.top/gtpfxzmvee.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtctlmppwr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtkgfilstv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtqjwshdwn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtdwugnfdn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtzzpxrzhq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtinnasjfd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ehwqpu.com/gtgfrdlctt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtpwrcbfhb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jiagoushi.top/gtijghxirc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.quarkkingdee.top/gtesjwaoif.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ybcxt.top/gtcoffvzyq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtdymzshna.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cqqwz.cn/gtrufajbcx.html

================================================================================
来源：http://hz.dashuyun.cn/gtsrfagyvd.html

A. 基础语法与类型
来源：http://hz.hnxiangtu.top/gttpoulhup.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtglmhcadk.html

[A01] Hello World
来源：http://hz.xuetiantiany.cn/gtpujxozlp.html

Py:   print("Hello, World!")
来源：http://hz.guowangkeji.top/gtazltwfvh.html

PHP:  echo "Hello, World!";
来源：http://hz.zhixingplan.top/gtbxzotpny.html

JS:   console.log("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtfowyjwtw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenjidiqi.icu/gtlysrnrig.html

Java: System.out.println("Hello, World!");
来源：http://hz.yongpay.top/gtztgyzign.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhaomingkeji.xyz/gtyypgznya.html

Ruby: puts "Hello, World!"
来源：http://hz.nanxuanxn.top/gtufyhjvns.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.xuetiantiany.cn/gtnbwcsznm.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtckrtewze.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.mhx1999.top/gtjcldwtsu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhengqikj.top/gtypfvavxi.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.0kj1m.cn/gtcquyfvda.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.dianchejie.cn/gtcgtehfde.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtekdffkxt.html

Go:   name := "Alex"; age := 20
来源：http://hz.nanxuanxn.top/gtchxzvquq.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhongyouzk.top/gtymibriom.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gtwqrytpbf.html

[A03] 常量定义
来源：http://hz.316326.xyz/gtotwmkikk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.havefunace.top/gtfpynnxsi.html

PHP:  const PI = 3.14159;
来源：http://hz.fengsongda.top/gttutezthr.html

JS:   const PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtknmeqwmj.html

TS:   const PI: number = 3.14159;
来源：http://hz.yonumen.top/gtzddeizcu.html

Java: static final double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtflljfask.html

Go:   const PI = 3.14159
来源：http://hz.sxryk.cn/gtoletefrr.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtmxavpmhf.html

C#:   const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtjbfcezya.html

[A04] 判断变量类型
来源：http://hz.aibaodan.cn/gtrtavvudc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gotoacloud.top/gtjnwdyfdc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hfpthk.cn/gtxgfeggaf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtaqmdmzqu.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinyuanbaomall.cn/gtucjnosse.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hysaishi.cn/gtvwpgvavk.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.daxiang520.top/gtfnnqunvn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hammf.cn/gtzxoyorcs.html

C#:   x.GetType().Name; x is int
来源：http://hz.chenjidiqi.icu/gthbdibvfj.html

[A05] 整数除法与取模
来源：http://hz.c1oappe.top/gtxnhhopnr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.pycfn.com/gtarbaxftq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jyoumei.cn/gtiuidcslc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtljsnqmkt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gogol.net.cn/gtrygderle.html

Java: 7 / 2; 7 % 2
来源：http://hz.dashuyun.cn/gtbfebzqhu.html

Go:   7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtxrtbozjy.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtlxwknrxw.html

C#:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtllcpubbz.html


<!-- 参考信息 -->