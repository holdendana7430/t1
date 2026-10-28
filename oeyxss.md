代发 wailian999

[U51] PHP：数组解构
来源：http://hz.ydzc1.top/gtktzcdjvj.html

[$a, $b] = $arr;
来源：http://hz.nanxinkj.top/gtjstrwoaf.html

[U52] PHP：箭头函数
来源：http://hz.zhoulong.xyz/gtupukfhnq.html

$double = fn($x) => $x * 2;
来源：http://hz.yanxiufei.cn/gttukabczf.html

[U53] PHP：空合并运算符
来源：http://hz.0kj1m.cn/gtgbqexzrj.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuetiantiany.cn/gtjspieihl.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtpsalxdzl.html

$obj?->method()
来源：http://hz.snrcjt.cn/gtkcoyaxea.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtgjyrovdn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtxiwgjmth.html

[U56] PHP：命名参数
来源：http://hz.quarkkingdee.top/gtnyyzrrvo.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gteztskivl.html

[U57] PHP：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtvetlpmww.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtlenxmhyc.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtmddkputl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.9152youxi.cn/gtseziesyb.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gtlcasuwjl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gthkcbqxhx.html

[U60] PHP：JSON 编解码
来源：http://hz.xinyue.icu/gtkimbjcah.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pengpengdd.cyou/gtmdkqurbv.html

[U61] PHP：正则
来源：http://hz.bjfxy.top/gtmhfrpgls.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtllezzvye.html

[U62] PHP：日期对象
来源：http://hz.gogol.net.cn/gtlnugjyvj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guowangkeji.top/gtkswhystp.html

[U63] PHP：文件读写
来源：http://hz.pengpengdd.cyou/gtqmgmuean.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ppjwa.cn/gtqekzpbvy.html

[U64] PHP：目录遍历
来源：http://hz.pycfn.com/gtqckftgqm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtfgefvfic.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtmcuypdwy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aibaodan.cn/gtankzxpoo.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtnsamnaas.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ivvv.top/gtlgarfwir.html

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gtaofsjurj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ppjwa.cn/gtzmugsnqc.html

[U68] PHP：PDO 连接
来源：http://hz.zhixingplan.top/gtvknghgkt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.svipenyu.cn/gtnfbrigds.html

[U69] PHP：PDO 预处理
来源：http://hz.fzhhl.top/gtwmsjlcvv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xziqi.cn/gtjcwwjiuz.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258888.top/gtsnggovnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtpixbvffl.html

[U71] PHP：抛出异常
来源：http://hz.yj202588.top/gtwtiilkum.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigfzy.top/gtimoffhoq.html

[U72] PHP：写错误日志
来源：http://hz.yvedp.cn/gtglnmmajw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhiwuduotai.top/gtrkisgtkp.html

[U73] PHP：读取 ini 配置
来源：http://hz.yanxiufei.cn/gtstxaetsg.html

parse_ini_file("config.ini", true)
来源：http://hz.kuanghao11.cn/gtmqrbqnig.html

[U74] PHP：读取环境变量
来源：http://hz.cdnleiting.top/gtagdradbc.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gaohongyu789.top/gtjrtogsre.html

[U75] PHP：依赖注入
来源：http://hz.gaohongyu789.top/gtgbtqfobv.html

composer require psr/container
来源：http://hz.gzhubu.top/gtttzowxoe.html

[U76] PHP：简单路由
来源：http://hz.shzxlz.cn/gtahfghrsz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.havefunace.top/gtcrzlibkg.html

[U77] PHP：模板渲染
来源：http://hz.yj20258888.top/gtlxvztmlp.html

composer require twig/twig
来源：http://hz.jinqigfzy.top/gtddbsntyn.html

[U78] PHP：单元测试
来源：http://hz.iojbl.cn/gtfabvgzug.html

composer require --dev phpunit/phpunit
来源：http://hz.hywenlv.cn/gtknhefaqq.html

[U79] PHP：静态分析
来源：http://hz.cdnleiting.top/gtwcqrlvvl.html

composer require --dev phpstan/phpstan
来源：http://hz.jinqigufen.top/gtufqjganz.html

[U80] PHP：代码规范修复
来源：http://hz.fengsongda.top/gtirfzmxqb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jiagoushi.top/gtkmxkanyj.html

[U81] JS：初始化项目
来源：http://hz.jyoumei.cn/gtxmazykcw.html

npm init -y;  npm i express
来源：http://hz.gogol.net.cn/gteqiaadvk.html

[U82] JS：package.json 脚本
来源：http://hz.zhoulong.xyz/gtfatcodpd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhiwuduotai.top/gtkbebwefm.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258888.top/gtvjovjvnb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jqgfzy.top/gtlaoqqbau.html

[U84] JS：CommonJS 写法
来源：http://hz.sweek.top/gtwfuhgunb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.birdmap.top/gtghnadlui.html

[U85] JS：可选链
来源：http://hz.xziqi.cn/gtvkboweki.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtslcffgle.html

[U86] JS：空值合并
来源：http://hz.nwbrower.top/gtqkhkljse.html

a ?? b
来源：http://hz.shanyushiyangkeji.top/gttvldcgfm.html

[U87] JS：解构默认值
来源：http://hz.yonumen.top/gtaqfqqwwh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj20258.top/gtjbachxdr.html

[U88] JS：对象展开合并
来源：http://hz.pycfn.com/gtkattsbqn.html

{ ...a, ...b }
来源：http://hz.redwolf501.top/gtxsgpaebo.html

[U89] JS：数组去重
来源：http://hz.fzhhl.top/gtvdvstrgp.html

[...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtowycktvk.html

[U90] JS：数字数组排序
来源：http://hz.yj20258.top/gtxciumfxu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtqvtxmlae.html

[U91] JS：对象键值遍历
来源：http://hz.gogol.net.cn/gtiyumhrer.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinyuanbaomall.cn/gtacrykznq.html

[U92] JS：深拷贝
来源：http://hz.yongpay.top/gtsmoojwjc.html

structuredClone(obj)
来源：http://hz.ehwqpu.com/gtcbjbupgj.html

[U93] JS：模板字符串
来源：http://hz.zhoulong.xyz/gtxfgpcuby.html

`共 ${n} 条`
来源：http://hz.yj20258.top/gtxtohyzjo.html

[U94] JS：箭头函数
来源：http://hz.shuidangran.top/gtjxtzylzt.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtylfdaxgt.html

[U95] JS：Promise 包装
来源：http://hz.yuanzhike.top/gtpgnwxgbf.html

new Promise((resolve, reject) => {})
来源：http://hz.cdnleiting.top/gtkuptohgt.html

[U96] JS：async/await 与异常
来源：http://hz.sufxvd.cn/gtaprftwtu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gteiekksdh.html

[U97] JS：并发请求
来源：http://hz.xinyue.icu/gtvhnwohcw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtjfccwytb.html

[U98] JS：fetch 带 JSON
来源：http://hz.snrcjt.cn/gtdqmmcslu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.snrcjt.cn/gtwjtrdyzr.html

[U99] JS：事件监听
来源：http://hz.jqgufenzy.top/gttcttkjkj.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtusmkdhzt.html

[U100] JS：DOM 查询
来源：http://hz.birdmap.top/gtzffnljaw.html

document.querySelector(".item")
来源：http://hz.yuanzhike.top/gtrhnetvyx.html

[U101] JS：classList 操作
来源：http://hz.zhixingplan.top/gtkhyuuexn.html

el.classList.toggle("active")
来源：http://hz.xylfe.cn/gtiemxkzlg.html

[U102] JS：本地存储
来源：http://hz.sufxvd.cn/gtzmqzwabr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jlsjyb.cn/gtmciqasog.html

[U103] JS：定时器
来源：http://hz.zycfv.cn/gtxoozfngy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuanzx.com/gtfvuijgkz.html

[U104] JS：防抖
来源：http://hz.hammf.cn/gtlfnpgxad.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtvagqfsls.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtcnxljzgh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sxryk.cn/gtrhzkzmoh.html

[U106] JS：日期格式化
来源：http://hz.xuanzx.com/gtkjzstusz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtdkmdywjs.html

[U107] JS：数字千分位
来源：http://hz.jinqigfzy.top/gtnnutrxqs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dashuyun.cn/gttflikbvc.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtmqmockpu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.pengpengdd.cyou/gttohzladz.html

[U109] JS：数组分组
来源：http://hz.52xcode.cn/gtmgpvzqpw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtryfjozhw.html

[U110] JS：数组分块
来源：http://hz.sufxvd.cn/gtfjrpjxsg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nanxuanxn.top/gtwldkivdu.html

[U111] JS：对象转 Map
来源：http://hz.guowangkeji.top/gtghiihlrq.html

new Map(Object.entries(obj))
来源：http://hz.wangshuangyany.cn/gtxppaqblz.html

[U112] JS：字符串补位
来源：http://hz.pycfn.com/gtynshkcei.html

"7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtfvxppvvh.html

[U113] JS：正则替换全部
来源：http://hz.jianghu66.top/gtcnelolsh.html

s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtmywqvldm.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtjdtxsdvl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtgbghncgn.html

[U115] JS：生成 UUID
来源：http://hz.yangfankeji.com/gtwjgcuwhw.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gtgtrwhgkj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sweek.top/gtvuvlfuki.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuanzhike.top/gtlabohgpx.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gtdjoupmyc.html

npm i -D vitest;  npx vitest
来源：http://hz.xylfe.cn/gtvsksmzeg.html

[U118] JS：开发服务器
来源：http://hz.hnqzz.top/gtpejyybkj.html

npm i -D vite;  npx vite
来源：http://hz.sxryk.cn/gtxlajcvuu.html

[U119] JS：生产构建
来源：http://hz.gogol.net.cn/gtdhploxfn.html

npx vite build
来源：http://hz.shanyushiyangkeji.top/gtrcpiqslj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtkglitbzq.html

import.meta.env.VITE_API_URL
来源：http://hz.yanxiufei.cn/gtkcmbwykl.html

================================================================================
来源：http://hz.gzhubu.top/gthzmyyacl.html

统计汇总
来源：http://hz.nwbrower.top/gtgoknmhad.html

================================================================================
来源：http://hz.tanke756.top/gtahmhqjby.html

按语言统计（条）：
来源：http://hz.birdmap.top/gtqrcfrgep.html

Python ......... 252
来源：http://hz.daxiang520.top/gtvwxbzbbx.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gtvtgaqxav.html

JavaScript ..... 252
来源：http://hz.hongshengwenyu.top/gtboslromw.html

TypeScript ..... 212
来源：http://hz.yuxming.cn/gtltwulfts.html

Java ........... 212
来源：http://hz.daxiang520.top/gtbsmymsgx.html

Go ............. 212
来源：http://hz.birdmap.top/gtrrppnmci.html

Ruby ........... 212
来源：http://hz.yuxming.cn/gtnrmskbcp.html

C# ............. 212
来源：http://hz.tanke756.top/gtjdqmpidf.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtcdkhthni.html

C++ ............ 30
来源：http://hz.yj20258.top/gttpjwwnzn.html

SQL ............ 90
来源：http://hz.xylfe.cn/gtrlrodqde.html

Bash ........... 80
来源：http://hz.shanyushiyangkeji.top/gtupheglpn.html

Kotlin ......... 15
来源：http://hz.316326.xyz/gtxlqxekqv.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtktkprrbu.html

Lua ............ 10
来源：http://hz.yvedp.cn/gtxxjykksv.html

Perl ........... 10
来源：http://hz.gzhubu.top/gtfrvzkhox.html

Scala .......... 10
来源：http://hz.chenlongwang.top/gtpaliuopz.html

------------------------------------
来源：http://hz.yuanzhike.top/gtlahuicdp.html

合计 ........... 2106 条
来源：http://hz.yj20258888.top/gtpkzeqebz.html

按章节统计：
来源：http://hz.zhoulong.xyz/gtryzqzsnf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtbolmzktn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtlroqfhap.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtphpqyojh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtdmvzczhk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ybcxt.top/gtkghunldv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtzszagvdx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtcxdtjmnt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.snrcjt.cn/gtpmlsvcog.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtquvspnpc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.sxryk.cn/gtwnwsjivi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtdrtnazbw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtgqdtoesk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtiyqbzswh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtjakelsyp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgfzy.top/gtykawfjpb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtmhvjifsu.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gthmydvbfa.html

R Bash 专题                             80
来源：http://hz.sufxvd.cn/gtdxojoemf.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtmoywhnyl.html

T 其他语言补充                          60
来源：http://hz.shanyushiyangkeji.top/gtuzyfjdbv.html

U 高频实用片段                         120
来源：http://hz.chenzaomai.com/gtdtwrgtgd.html

------------------------------------
来源：http://hz.jinqigufen.top/gtayalovbk.html

合计                                  2106 条
来源：http://hz.ybcxt.top/gtlqmleekg.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtwwyzztud.html

使用提醒
来源：http://hz.xinyue.icu/gtjuwwszmi.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtrstuyiik.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yj202588.top/gtagzfghdh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sysykeji.top/gtkknvkunn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj20258.top/gtdeasuwnn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yvedp.cn/gtavrsgqfy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.meibo888.top/gtabyiobht.html

—— 文件结束 ——
来源：http://hz.cqqwz.cn/gticguylvj.html

================================================================================
来源：http://hz.316326.xyz/gtertaetfv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jlsjyb.cn/gthmmfxpim.html

Common Programming Examples Cheat Book
来源：http://hz.zhaomingkeji.xyz/gtsaflpkss.html

================================================================================
来源：http://hz.nwbrower.top/gtwiuarfmv.html

【收录内容】
来源：http://hz.sweek.top/gtoniptkyy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtrynwkxok.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.nanxinkj.top/gtawfhhkzr.html

SQL · Bash · C · C++
来源：http://hz.sysykeji.top/gthmdhvece.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cqqwz.cn/gtfptefcwb.html

【使用说明】
来源：http://hz.hnqzz.top/gtfklrpkmh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhaomingkeji.xyz/gtaiqwzrae.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jqgufenzy.top/gtdhudvmgo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydjk.org.cn/gtnmvzprsz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.andypj.xyz/gtlndsqpkd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.316326.xyz/gtcbnysrtk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.guowangkeji.top/gtxssobalp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangtech.top/gtjcuvadhe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.quarkkingdee.top/gtcglwhbcr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cucudq.cn/gtxhtcantm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jlsjyb.cn/gtkvkpwofj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yonumen.top/gtnifbesoa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hfpthk.cn/gtdcunizld.html

【文件统计】
来源：http://hz.andypj.xyz/gtlnslqvai.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.vqdsnc.cn/gtuohusgxn.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtuukqwyxc.html

目  录
来源：http://hz.gzhubu.top/gtcudlznur.html

--------------------------------------------------------------------------------
来源：http://hz.tian-w.cn/gtealqmrew.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhixingplan.top/gtvjzwxkkw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtxrdrjtie.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtmyagpqei.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtbexbmvvw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.316326.xyz/gtvuuxzsps.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtrtzrnbrx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.birdmap.top/gtvwvmfjow.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hysaishi.cn/gtrhnavobh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtaqnksncx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tianlin.xyz/gtnbythuvh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtrgcrjwxa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtlgwkiayp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gthcylxybv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.dianchejie.cn/gtudivdvsk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yangfankeji.com/gtfdifyryd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtibacrqzz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gogol.net.cn/gtkkdqhbku.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xylfe.cn/gtryevyqoo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.9152youxi.cn/gtldfdpmpk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtrvuhqisa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtpxacxugz.html

================================================================================
来源：http://hz.jianghu66.top/gtshoyfqfw.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gttiumdhmg.html

================================================================================
来源：http://hz.hfpthk.cn/gtkuxnsuii.html

[A01] Hello World
来源：http://hz.dashuyun.cn/gtkvnnmgmp.html

Py:   print("Hello, World!")
来源：http://hz.yangfankeji.com/gtswjwlmvc.html

PHP:  echo "Hello, World!";
来源：http://hz.sxryk.cn/gtrduvotmp.html

JS:   console.log("Hello, World!");
来源：http://hz.zhijiandao.cn/gtvqooyugt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hfpthk.cn/gtwyliqyyp.html

Java: System.out.println("Hello, World!");
来源：http://hz.quarkkingdee.top/gtrzjfosan.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.iojbl.cn/gtffmwffyc.html

Ruby: puts "Hello, World!"
来源：http://hz.meibo888.top/gtzspthipz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtmiqttcbl.html

[A02] 变量声明与赋值
来源：http://hz.tian-w.cn/gtwxoboquo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuanzx.com/gtcjovnytq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nwbrower.top/gtofcvorea.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.aibaodan.cn/gtnyjijgij.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ppjwa.cn/gtvuotyqpn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtbyovxcmo.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhengqikj.top/gtrlsdaahz.html

Ruby: name = "Alex"; age = 20
来源：http://hz.svipenyu.cn/gtobhtpvkt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gtkjcapsus.html

[A03] 常量定义
来源：http://hz.jyoumei.cn/gtlklmfhuy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xuetiantiany.cn/gtsdldemcy.html

PHP:  const PI = 3.14159;
来源：http://hz.fengsongda.top/gtodxanezd.html

JS:   const PI = 3.14159;
来源：http://hz.chenzaomai.com/gtauissydc.html

TS:   const PI: number = 3.14159;
来源：http://hz.yj20258.top/gtybrvmody.html

Java: static final double PI = 3.14159;
来源：http://hz.ybcxt.top/gtzypaerie.html

Go:   const PI = 3.14159
来源：http://hz.quarkkingdee.top/gtqobrssrz.html

Ruby: PI = 3.14159
来源：http://hz.c1oappe.top/gtdoxthjsg.html

C#:   const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtjgpfhoif.html

[A04] 判断变量类型
来源：http://hz.xingfuxueyuan.xyz/gtfbmofwrb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jlsjyb.cn/gtjdyljeyo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yueranfly.top/gtnceggrka.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangtech.top/gthaufpsin.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnxiangtu.top/gtbscmikjd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gogol.net.cn/gtyzhakkds.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gaohongyu789.top/gtdxefawlr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhengqikj.top/gtfolscdnk.html

C#:   x.GetType().Name; x is int
来源：http://hz.9152youxi.cn/gtivvzpewy.html

[A05] 整数除法与取模
来源：http://hz.chenlongwang.top/gtrlmzqjcf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xuetiantiany.cn/gtyemudtqy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtcehhhmjd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuanzx.com/gtbfybgmqv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtlvklvkbh.html

Java: 7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtclgvejjv.html

Go:   7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtjiqpjroi.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtrmrubhhj.html

C#:   7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtujscidgu.html

[A06] 字符串转数字
来源：http://hz.sweek.top/gtkwzxkynv.html

Py:   int("42"); float("3.14")
来源：http://hz.meibo888.top/gtgsebxujl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yj20258888.top/gtrxhwpwxh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.daria6918.cn/gtxlvskezf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.daria6918.cn/gtoyahhxai.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.sxryk.cn/gtnocxcwrm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.shanyushiyangkeji.top/gtilrvadiu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xuanzx.com/gtngefkvjc.html


<!-- 参考信息 -->