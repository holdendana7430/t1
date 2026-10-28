代发 wailian999

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gtsihpiffq.html

[$a, $b] = $arr;
来源：http://hz.ybcxt.top/gtzuyednnd.html

[U52] PHP：箭头函数
来源：http://hz.zhixingplan.top/gtqivbnfjm.html

$double = fn($x) => $x * 2;
来源：http://hz.ydzc1.top/gtwseoqxoe.html

[U53] PHP：空合并运算符
来源：http://hz.chenjidiqi.icu/gtsufkukiv.html

$v = $a ?? $b ?? "default";
来源：http://hz.ywan-chungtsiang.top/gtmznvhlfe.html

[U54] PHP：空安全调用
来源：http://hz.52xcode.cn/gtausfqvyx.html

$obj?->method()
来源：http://hz.shuidangran.top/gtyvkbmpgq.html

[U55] PHP：match 表达式
来源：http://hz.jiagoushi.top/gtpxrjilid.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.pycfn.com/gtpedxvkiq.html

[U56] PHP：命名参数
来源：http://hz.dianchejie.cn/gtvrxoanvj.html

f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtdwxxcqwp.html

[U57] PHP：字符串插值
来源：http://hz.0kj1m.cn/gtptrflnmo.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtkwhgumjq.html

[U58] PHP：数组三件套
来源：http://hz.svipenyu.cn/gtuggydczp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigfzy.top/gthijtvpcc.html

[U59] PHP：自定义排序
来源：http://hz.xinyue.icu/gtmawprfte.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtvmerwtzj.html

[U60] PHP：JSON 编解码
来源：http://hz.jinghuilouyu.cn/gtjyyozxyr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yangfankeji.com/gtraoalhps.html

[U61] PHP：正则
来源：http://hz.yongpay.top/gtnxohfvxr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xylfe.cn/gthdyzggaq.html

[U62] PHP：日期对象
来源：http://hz.meibo888.top/gtoogrlbsm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuxming.cn/gtdiqgnnoz.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtzdzijyad.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gttpmmrfnc.html

[U64] PHP：目录遍历
来源：http://hz.jinqigufen.top/gtjzbzocdd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinqigfzy.top/gtebipuhwz.html

[U65] PHP：会话
来源：http://hz.cucudq.cn/gtkvbhsdmm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtvjqukcnk.html

[U66] PHP：设置 Cookie
来源：http://hz.mhx1999.top/gtettppwqn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj202588.top/gtoejzwtvh.html

[U67] PHP：处理文件上传
来源：http://hz.pycfn.com/gtzqadbdcp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pengpengdd.cyou/gtbzzagqij.html

[U68] PHP：PDO 连接
来源：http://hz.yonumen.top/gtzktaxczp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.dashuyun.cn/gtsiygekky.html

[U69] PHP：PDO 预处理
来源：http://hz.jqgufenzy.top/gtdebeterq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj202588.top/gtssuheawi.html

[U70] PHP：PDO 事务
来源：http://hz.9152youxi.cn/gtopqrzszg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.c1oappe.top/gtunsgjlni.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtsvmzfkch.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258.top/gtfmzbqimc.html

[U72] PHP：写错误日志
来源：http://hz.hongshengwenyu.top/gtqujoeytw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tanke756.top/gtlzcrlspd.html

[U73] PHP：读取 ini 配置
来源：http://hz.guowangkeji.top/gtmkimqjdv.html

parse_ini_file("config.ini", true)
来源：http://hz.wangdashe.top/gtdnuwhmpi.html

[U74] PHP：读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtumnjiubb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinqigufen.top/gtyvjzrpll.html

[U75] PHP：依赖注入
来源：http://hz.guannengcc.top/gtqnbnkjyu.html

composer require psr/container
来源：http://hz.chenzaomai.com/gtfjnweuhr.html

[U76] PHP：简单路由
来源：http://hz.cucudq.cn/gtnkwisntb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zycfv.cn/gtfxumddii.html

[U77] PHP：模板渲染
来源：http://hz.nanxuanxn.top/gtchgqfyil.html

composer require twig/twig
来源：http://hz.zhijiandao.cn/gttdqduupm.html

[U78] PHP：单元测试
来源：http://hz.vqdsnc.cn/gtuoouptpv.html

composer require --dev phpunit/phpunit
来源：http://hz.jlsjyb.cn/gtuoozqkhw.html

[U79] PHP：静态分析
来源：http://hz.yueranfly.top/gtqlrzdpuf.html

composer require --dev phpstan/phpstan
来源：http://hz.vqdsnc.cn/gtmjvhiish.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtoetkabjn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.haohaochexian.top/gtkmdashvb.html

[U81] JS：初始化项目
来源：http://hz.yanxiufei.cn/gturzszqav.html

npm init -y;  npm i express
来源：http://hz.zhaomingkeji.xyz/gtfyfijccw.html

[U82] JS：package.json 脚本
来源：http://hz.xuanzx.com/gtoofhtlkf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tian-w.cn/gtfjdnbhsa.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhijiandao.cn/gtjvpqeouv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.9152youxi.cn/gtnwmjpgyr.html

[U84] JS：CommonJS 写法
来源：http://hz.andypj.xyz/gtcasasfsm.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tian-w.cn/gtlzyctftd.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gthnnyutyo.html

a?.b?.c
来源：http://hz.hysaishi.cn/gtvzgztehn.html

[U86] JS：空值合并
来源：http://hz.yongpay.top/gttxaiofri.html

a ?? b
来源：http://hz.yuxming.cn/gtaviqpahb.html

[U87] JS：解构默认值
来源：http://hz.svipenyu.cn/gtilzbehrx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sxryk.cn/gtttgtqcni.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtspevidie.html

{ ...a, ...b }
来源：http://hz.xingfuxueyuan.xyz/gtvcfbzyaf.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtivimkjbb.html

[...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtktrcixec.html

[U90] JS：数字数组排序
来源：http://hz.sysykeji.top/gtnrjsnwvg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtmeezjdid.html

[U91] JS：对象键值遍历
来源：http://hz.yuanzhike.top/gtaceonxgn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sufxvd.cn/gtyqbpoqcg.html

[U92] JS：深拷贝
来源：http://hz.zhijiandao.cn/gthorxyfuw.html

structuredClone(obj)
来源：http://hz.iojbl.cn/gtcjdoogqe.html

[U93] JS：模板字符串
来源：http://hz.gogol.net.cn/gtmgdvusyd.html

`共 ${n} 条`
来源：http://hz.redwolf501.top/gtizgzygwy.html

[U94] JS：箭头函数
来源：http://hz.bjfxy.top/gtffdtuirf.html

const double = x => x * 2;
来源：http://hz.zhengqikj.top/gtxtnziigk.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtmcaxzyra.html

new Promise((resolve, reject) => {})
来源：http://hz.feifeiyinyue.top/gtzohkwkfg.html

[U96] JS：async/await 与异常
来源：http://hz.quarkkingdee.top/gtqvqpbssj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtvzmkyfhu.html

[U97] JS：并发请求
来源：http://hz.aibaodan.cn/gtnfdzbqsn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gthrxdbblr.html

[U98] JS：fetch 带 JSON
来源：http://hz.yueranfly.top/gthluaixvm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hnxiangtu.top/gtdwxiycti.html

[U99] JS：事件监听
来源：http://hz.andypj.xyz/gtkneyuhcw.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtjuppoyae.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtxpcbdokf.html

document.querySelector(".item")
来源：http://hz.yangfankeji.com/gtjwvuxxcn.html

[U101] JS：classList 操作
来源：http://hz.gaohongyu789.top/gteqwqfbdy.html

el.classList.toggle("active")
来源：http://hz.hnxiangtu.top/gtsamnthjw.html

[U102] JS：本地存储
来源：http://hz.haohaochexian.top/gtrbznqpvq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.316326.xyz/gtkbzvkard.html

[U103] JS：定时器
来源：http://hz.jiagoushi.top/gtewlfergw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tianlin.xyz/gtlwtyflij.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtbzmjiqjy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtxewgjhep.html

[U105] JS：节流
来源：http://hz.nanxinkj.top/gtvhulpipe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.guowangkeji.top/gtepeldpeq.html

[U106] JS：日期格式化
来源：http://hz.hongshengwenyu.top/gtexvoujne.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.vqdsnc.cn/gtbllqvxyo.html

[U107] JS：数字千分位
来源：http://hz.xuetiantiany.cn/gtxfqxrosv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxuanxn.top/gttnfhikbs.html

[U108] JS：随机整数
来源：http://hz.xuanzx.com/gtepytkuln.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydzc1.top/gtgiqhpihs.html

[U109] JS：数组分组
来源：http://hz.nanxinkj.top/gtoddhffnr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtlbirujuy.html

[U110] JS：数组分块
来源：http://hz.hnxiangtu.top/gtcfjrwxzl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zdqjudy.top/gtwtaymlwc.html

[U111] JS：对象转 Map
来源：http://hz.xinyue.icu/gtrhnldccu.html

new Map(Object.entries(obj))
来源：http://hz.gogol.net.cn/gttxcgwxxj.html

[U112] JS：字符串补位
来源：http://hz.xylfe.cn/gtbhvwqcjh.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtwodhnrwb.html

[U113] JS：正则替换全部
来源：http://hz.zycfv.cn/gtpcfpnrnp.html

s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtplpfkpgw.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258888.top/gtnezamdvn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gttqvugydk.html

[U115] JS：生成 UUID
来源：http://hz.hfpthk.cn/gtbosbzalo.html

crypto.randomUUID()
来源：http://hz.tian-w.cn/gtnftkwjlf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hfpthk.cn/gtirrkwryq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtpvwnaffv.html

[U117] JS：单元测试
来源：http://hz.yj202588.top/gtiqimhiti.html

npm i -D vitest;  npx vitest
来源：http://hz.hammf.cn/gtovchrjdn.html

[U118] JS：开发服务器
来源：http://hz.yj20258888.top/gtltiwwyxd.html

npm i -D vite;  npx vite
来源：http://hz.gaohongyu789.top/gtgnxykeov.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtlfpqoiwb.html

npx vite build
来源：http://hz.jqgufenzy.top/gtsxwyzydy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daxiang520.top/gtcqeerppx.html

import.meta.env.VITE_API_URL
来源：http://hz.dianchejie.cn/gtubulqxjn.html

================================================================================
来源：http://hz.cheryme.top/gtleslukgn.html

统计汇总
来源：http://hz.shanyushiyangkeji.top/gtimbcnfna.html

================================================================================
来源：http://hz.hnxiangtu.top/gtgkripvdz.html

按语言统计（条）：
来源：http://hz.dashuyun.cn/gtzxnirnom.html

Python ......... 252
来源：http://hz.daxiang520.top/gtrxwvlioz.html

PHP ............ 252
来源：http://hz.jinyuanbaomall.cn/gtjwqfwzdo.html

JavaScript ..... 252
来源：http://hz.tanke756.top/gtigxqazwx.html

TypeScript ..... 212
来源：http://hz.aibaodan.cn/gtmujlukhz.html

Java ........... 212
来源：http://hz.xinyue.icu/gtonrazvkt.html

Go ............. 212
来源：http://hz.shuidangran.top/gtcnzxgovx.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtqdkmeero.html

C# ............. 212
来源：http://hz.haohaochexian.top/gtosrpupnl.html

C .............. 30
来源：http://hz.cheryme.top/gttviurrnu.html

C++ ............ 30
来源：http://hz.hongshengwenyu.top/gtyxovjbru.html

SQL ............ 90
来源：http://hz.zhongyouzk.top/gtgsjbjjnf.html

Bash ........... 80
来源：http://hz.cdnleiting.top/gtvfsjxhql.html

Kotlin ......... 15
来源：http://hz.yuanzhike.top/gtbrbnkyda.html

Swift .......... 15
来源：http://hz.yueranfly.top/gtshcfhfok.html

Lua ............ 10
来源：http://hz.yuanzhike.top/gtdvqpapxe.html

Perl ........... 10
来源：http://hz.cheryme.top/gtswrfddce.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gtsequpzee.html

------------------------------------
来源：http://hz.yanxiufei.cn/gtgapkncha.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gttenumvup.html

按章节统计：
来源：http://hz.smart0.xyz/gtzdgxazcs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtnocarcfy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtpdcuwmxv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtncvejwvp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtwobshckt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yuanzhike.top/gtjcrtbtbx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtiyawhzob.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtgrnrybdn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtpwlgsbcr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtpwuuiftp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtvozdmdra.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtvhniszyi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtktxuagdh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtslkflhof.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtcouvzovv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.9152youxi.cn/gtpmbzmqjk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtalcsosnp.html

Q SQL 专题                              90
来源：http://hz.zhiwuduotai.top/gtrqvblxbz.html

R Bash 专题                             80
来源：http://hz.zhiwuduotai.top/gtighrtvdf.html

S C / C++ 专题                          60
来源：http://hz.yj20258888.top/gtauagwghr.html

T 其他语言补充                          60
来源：http://hz.yvedp.cn/gtsienrkhv.html

U 高频实用片段                         120
来源：http://hz.daria6918.cn/gtxmjxygaz.html

------------------------------------
来源：http://hz.bjfxy.top/gtnntmfupi.html

合计                                  2106 条
来源：http://hz.yonumen.top/gtywdwidul.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtklttwhdn.html

使用提醒
来源：http://hz.cheryme.top/gtryudqibu.html

--------------------------------------------------------------------------------
来源：http://hz.smart0.xyz/gtutswqkas.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yongpay.top/gtbubnizeq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hongshengwenyu.top/gtozrvqhfu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yuanzhike.top/gtzkxdaoez.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xingfuxueyuan.xyz/gtgcfzxlvl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ybcxt.top/gtznovjkpl.html

—— 文件结束 ——
来源：http://hz.zhixingplan.top/gtvbnwvjnq.html

================================================================================
来源：http://hz.dashuyun.cn/gtcuwyqcmr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.kuanghao11.cn/gtyirwmmmm.html

Common Programming Examples Cheat Book
来源：http://hz.snrcjt.cn/gtmxfqszco.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxmifemie.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtujjrozzz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shuidangran.top/gtagawkkbv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jyoumei.cn/gtgnpdaenq.html

SQL · Bash · C · C++
来源：http://hz.xuetiantiany.cn/gtmknspzlp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ivvv.top/gtdnzoxcri.html

【使用说明】
来源：http://hz.fengsongda.top/gtepfhhxda.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhixingplan.top/gtbfzedwop.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gaohongyu789.top/gtayiiniic.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jianghu66.top/gtvsfvoiym.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jyoumei.cn/gtzzswpwfo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jlsjyb.cn/gtuofbxvvb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtwplbtwgh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.tian-w.cn/gtyreyaqjs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.shzxlz.cn/gtswosltzq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj20258888.top/gtjicvkncs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gtzkmqxpir.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yj202588.top/gtnozaborh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sysykeji.top/gtuwgnpqby.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtclbneytp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.smart0.xyz/gtxzdegvbq.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtpefttjgy.html

目  录
来源：http://hz.ydzc1.top/gtikaeeeui.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtfdyzjigu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinghuilouyu.cn/gtvslpgphe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtydvtwyur.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gttwkpfolt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gttooctqey.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.fzhhl.top/gtaetzjoph.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtropftudn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtlgogetod.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtndsloqno.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhongyouzk.top/gtrbcxckjo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.aibaodan.cn/gterrdhokv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtpumpgdzf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtftlxbmfx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gtrotvwgyd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.xingfuxueyuan.xyz/gttswbklrh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.wangshuangyany.cn/gtnlsqudru.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtqhfcnxih.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xingfuxueyuan.xyz/gtbruzrbee.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.mhx1999.top/gtxnfdzgjf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ydzc1.top/gtrvxyymms.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gtlphkpxtx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.guannengcc.top/gtgbkcabuk.html

================================================================================
来源：http://hz.svipenyu.cn/gtdbhsmgpb.html

A. 基础语法与类型
来源：http://hz.gogol.net.cn/gtubihijhw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtihpqkobh.html

[A01] Hello World
来源：http://hz.shzxlz.cn/gtjctnpcsa.html

Py:   print("Hello, World!")
来源：http://hz.guannengcc.top/gtlyuqpuoq.html

PHP:  echo "Hello, World!";
来源：http://hz.yangfankeji.com/gtqzbmxoor.html

JS:   console.log("Hello, World!");
来源：http://hz.jinghuilouyu.cn/gttptlmidm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.vqdsnc.cn/gtiuvkgret.html

Java: System.out.println("Hello, World!");
来源：http://hz.havefunace.top/gtveueuuga.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtjuftvria.html

Ruby: puts "Hello, World!"
来源：http://hz.chenzaomai.com/gthmfwfsls.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.redwolf501.top/gtgwkgomwk.html

[A02] 变量声明与赋值
来源：http://hz.shangyingyoupin.top/gtejgkgbly.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.birdmap.top/gthfwyrlid.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fzhhl.top/gttdaczntc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.snrcjt.cn/gtzhknieii.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cashguo.top/gtvbfrijmk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shuidangran.top/gtiezzpmkl.html

Go:   name := "Alex"; age := 20
来源：http://hz.xuetiantiany.cn/gtrucperye.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guowangkeji.top/gtrpzqdgzy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.guowangkeji.top/gtpdmvcjqe.html

[A03] 常量定义
来源：http://hz.yj20258888.top/gtsbafpdks.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sweek.top/gttaigdohh.html

PHP:  const PI = 3.14159;
来源：http://hz.ehwqpu.com/gtbrletleb.html

JS:   const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtwbpgtgox.html

TS:   const PI: number = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtxwbzlmxy.html

Java: static final double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtjgxtknou.html

Go:   const PI = 3.14159
来源：http://hz.cucudq.cn/gtmnnlicbz.html

Ruby: PI = 3.14159
来源：http://hz.hfpthk.cn/gtdiriuewn.html

C#:   const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtnxxeqzkt.html

[A04] 判断变量类型
来源：http://hz.wangshuangyany.cn/gtipklkgzw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gaohongyu789.top/gtothxslub.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj202588.top/gtdtudjfva.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cqqwz.cn/gtmeqhshlv.html

TS:   typeof x; x instanceof Date
来源：http://hz.0kj1m.cn/gthtzgwrxo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.wangdashe.top/gtijiynqxx.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.guowangkeji.top/gtbtuydeof.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cucudq.cn/gthgxjdmtq.html

C#:   x.GetType().Name; x is int
来源：http://hz.aibaodan.cn/gtyjargmaq.html

[A05] 整数除法与取模
来源：http://hz.svipenyu.cn/gtvkfqwttc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.quarkkingdee.top/gtubvkursy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jqgufenzy.top/gtjaocvshy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daxiang520.top/gtuumbbbae.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.nanxinkj.top/gtnwthqwuq.html

Java: 7 / 2; 7 % 2
来源：http://hz.52xcode.cn/gtvxqmdtcy.html

Go:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtwtsjfvgu.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sufxvd.cn/gtvgwiboxm.html

C#:   7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtahgyqarw.html

[A06] 字符串转数字
来源：http://hz.cheryme.top/gtostqkzms.html

Py:   int("42"); float("3.14")
来源：http://hz.xuanzx.com/gtjbrjqkjb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yangfankeji.com/gtjrwyifjg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hongshengwenyu.top/gtxrleslgg.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ydjk.org.cn/gtkybgunzs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.aibaodan.cn/gttxznirvy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.ivvv.top/gtwazbxaju.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gotoacloud.top/gtegpipglr.html


<!-- 参考信息 -->