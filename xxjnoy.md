代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hz.kuanghao11.cn/gtfnpadhpf.html

sys.stdout.isatty()
来源：http://hz.sysykeji.top/gtddptpylr.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtfmoeultn.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtatkvglpf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydzc1.top/gtbvtxpllr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtpmltoejw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guannengcc.top/gtifludphl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jianghu66.top/gtxptlfugu.html

[U43] PHP：声明命名空间
来源：http://hz.cdnleiting.top/gtvzgdnfmp.html

namespace App\Http;
来源：http://hz.tianlin.xyz/gttngbgudq.html

[U44] PHP：开启严格类型
来源：http://hz.yongpay.top/gtgfktywzd.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gtqyqtirec.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gtfuifdwxw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtybkhnszs.html

[U46] PHP：可空类型
来源：http://hz.shangyingyoupin.top/gtcnbfysys.html

?string $name = null
来源：http://hz.yonumen.top/gtfpmifovg.html

[U47] PHP：联合类型
来源：http://hz.jinqigufen.top/gtfuuqwjhl.html

int|string $id
来源：http://hz.c1oappe.top/gtexjqzsxv.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gtunvxteih.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.0kj1m.cn/gttpulglfe.html

[U49] PHP：只读属性
来源：http://hz.jianghu66.top/gtsaqdffsg.html

public readonly string $name
来源：http://hz.daria6918.cn/gtjeveixjd.html

[U50] PHP：构造器属性提升
来源：http://hz.gogol.net.cn/gtorjiowxq.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gttobcxopk.html

[U51] PHP：数组解构
来源：http://hz.xuetiantiany.cn/gthobdnlnm.html

[$a, $b] = $arr;
来源：http://hz.yongpay.top/gtagombvtp.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtixozmtdz.html

$double = fn($x) => $x * 2;
来源：http://hz.pengpengdd.cyou/gtmtgsdjki.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gtcgvlttzi.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtrhouwici.html

[U54] PHP：空安全调用
来源：http://hz.cheryme.top/gtdoatbozn.html

$obj?->method()
来源：http://hz.jinqigfzy.top/gtnzaecnaa.html

[U55] PHP：match 表达式
来源：http://hz.zhengqikj.top/gtewdvptoj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinghuilouyu.cn/gtbwhlkswu.html

[U56] PHP：命名参数
来源：http://hz.0kj1m.cn/gtkboxgifh.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtnmtyjdod.html

[U57] PHP：字符串插值
来源：http://hz.ppjwa.cn/gtukiykjue.html

"值: {$a}"
来源：http://hz.xinyue.icu/gtawtdxipq.html

[U58] PHP：数组三件套
来源：http://hz.zdqjudy.top/gtbehvfyvd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhongyouzk.top/gtizjgemrd.html

[U59] PHP：自定义排序
来源：http://hz.shangyingyoupin.top/gthtxutmsn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtqemvensk.html

[U60] PHP：JSON 编解码
来源：http://hz.yangfankeji.com/gtuancgwed.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.redwolf501.top/gtfaeelyiw.html

[U61] PHP：正则
来源：http://hz.xuetiantiany.cn/gttrqmteub.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gttaufsbnr.html

[U62] PHP：日期对象
来源：http://hz.kuanghao11.cn/gtkkpiigfg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ppjwa.cn/gtblmdindq.html

[U63] PHP：文件读写
来源：http://hz.xziqi.cn/gtwacxsqez.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj202588.top/gtehzdrsfw.html

[U64] PHP：目录遍历
来源：http://hz.yj202588.top/gtceehczaq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guowangkeji.top/gtbhocowjv.html

[U65] PHP：会话
来源：http://hz.gotoacloud.top/gtwngrevmk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.kuanghao11.cn/gtgrnmrnqi.html

[U66] PHP：设置 Cookie
来源：http://hz.aibaodan.cn/gtfkabwfki.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtnlozkunr.html

[U67] PHP：处理文件上传
来源：http://hz.ehwqpu.com/gtvoaouxiy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hammf.cn/gtpzsfkwfb.html

[U68] PHP：PDO 连接
来源：http://hz.chenlongwang.top/gtyylfnywg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sufxvd.cn/gtrnnuikgb.html

[U69] PHP：PDO 预处理
来源：http://hz.xuetiantiany.cn/gthcfomhlg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtuyzmkait.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtmlrzdzej.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hfpthk.cn/gtiixxlqka.html

[U71] PHP：抛出异常
来源：http://hz.hfpthk.cn/gtuuvlrgmm.html

throw new RuntimeException("失败", 500);
来源：http://hz.ydjk.org.cn/gtjugufeyw.html

[U72] PHP：写错误日志
来源：http://hz.tian-w.cn/gtzfpzuakl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sweek.top/gtipsivxww.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtzqhellwp.html

parse_ini_file("config.ini", true)
来源：http://hz.c1oappe.top/gtonnhvcdx.html

[U74] PHP：读取环境变量
来源：http://hz.gogol.net.cn/gtkqeyxmhw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.birdmap.top/gtgwkxoqbk.html

[U75] PHP：依赖注入
来源：http://hz.ppjwa.cn/gtfbnwmcxf.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtrmnmneza.html

[U76] PHP：简单路由
来源：http://hz.chenlongwang.top/gtiomdyyik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jqgufenzy.top/gtxnwerymj.html

[U77] PHP：模板渲染
来源：http://hz.iojbl.cn/gtpbdnyxfi.html

composer require twig/twig
来源：http://hz.daria6918.cn/gtyrntckeh.html

[U78] PHP：单元测试
来源：http://hz.jinqigufen.top/gteeuqspcs.html

composer require --dev phpunit/phpunit
来源：http://hz.gogol.net.cn/gtjnoouklf.html

[U79] PHP：静态分析
来源：http://hz.jinqigfzy.top/gtmdpxgnac.html

composer require --dev phpstan/phpstan
来源：http://hz.daria6918.cn/gttsnldyjz.html

[U80] PHP：代码规范修复
来源：http://hz.birdmap.top/gtyusndjgf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.meibo888.top/gtaojrlkxg.html

[U81] JS：初始化项目
来源：http://hz.yuxming.cn/gtppptbafo.html

npm init -y;  npm i express
来源：http://hz.xylfe.cn/gtzvashyhi.html

[U82] JS：package.json 脚本
来源：http://hz.cheryme.top/gtzbucdqmr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinqigufen.top/gtuclrrypc.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtlzqdotbd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cashguo.top/gtixuonvyu.html

[U84] JS：CommonJS 写法
来源：http://hz.jianghu66.top/gtmgejzubn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.guowangkeji.top/gtulaxmiqn.html

[U85] JS：可选链
来源：http://hz.gotoacloud.top/gtyblhmphp.html

a?.b?.c
来源：http://hz.jianghu66.top/gtkphvxlkg.html

[U86] JS：空值合并
来源：http://hz.shuidangran.top/gtkyzxzfhf.html

a ?? b
来源：http://hz.mhx1999.top/gtmnlssjis.html

[U87] JS：解构默认值
来源：http://hz.shuidangran.top/gtzqkmpitw.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ppjwa.cn/gttfzcpcyk.html

[U88] JS：对象展开合并
来源：http://hz.feifeiyinyue.top/gtasegaqxl.html

{ ...a, ...b }
来源：http://hz.daria6918.cn/gtmntzlzyy.html

[U89] JS：数组去重
来源：http://hz.cashguo.top/gtgbslnpqr.html

[...new Set(arr)]
来源：http://hz.cheryme.top/gtkwjhmiwd.html

[U90] JS：数字数组排序
来源：http://hz.sufxvd.cn/gtrujwxqcl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtixsnegaf.html

[U91] JS：对象键值遍历
来源：http://hz.snrcjt.cn/gtptwkwulk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenzaomai.com/gtccwlcfsa.html

[U92] JS：深拷贝
来源：http://hz.iojbl.cn/gtpmlznxrv.html

structuredClone(obj)
来源：http://hz.yangfankeji.com/gtgdjdfzar.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtzunqppps.html

`共 ${n} 条`
来源：http://hz.xylfe.cn/gtfeuestnw.html

[U94] JS：箭头函数
来源：http://hz.ydzc1.top/gtrfahkugv.html

const double = x => x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtgttnvbwp.html

[U95] JS：Promise 包装
来源：http://hz.jinghuilouyu.cn/gtwobfgidx.html

new Promise((resolve, reject) => {})
来源：http://hz.yvedp.cn/gtuycqkptz.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtmcnlltux.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtthwgynzn.html

[U97] JS：并发请求
来源：http://hz.dianchejie.cn/gtamljkcud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gthexmwmpz.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuetiantiany.cn/gtwtlzdocf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuxming.cn/gteghubnig.html

[U99] JS：事件监听
来源：http://hz.0kj1m.cn/gtatxvpkgj.html

el.addEventListener("click", e => {})
来源：http://hz.svipenyu.cn/gtwdthkbrb.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtphuzgrtw.html

document.querySelector(".item")
来源：http://hz.yj20258888.top/gtzgbdogam.html

[U101] JS：classList 操作
来源：http://hz.ybcxt.top/gtednwnzqr.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtjaadjrrv.html

[U102] JS：本地存储
来源：http://hz.gaohongyu789.top/gtygekyefh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gtxbrtaosi.html

[U103] JS：定时器
来源：http://hz.jyoumei.cn/gtukatzmit.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hammf.cn/gtmmgranab.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtowuvasnv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtknmygidg.html

[U105] JS：节流
来源：http://hz.nanxuanxn.top/gtbpamvsyr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtoojcayxk.html

[U106] JS：日期格式化
来源：http://hz.redwolf501.top/gtjfwdxlqr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.pycfn.com/gtlbvrkgto.html

[U107] JS：数字千分位
来源：http://hz.pengpengdd.cyou/gtqzbbyppm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtbywwjnzi.html

[U108] JS：随机整数
来源：http://hz.xylfe.cn/gtmgvmtbcn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtljxkdwwu.html

[U109] JS：数组分组
来源：http://hz.shzxlz.cn/gtzftwlmea.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtwfppbatu.html

[U110] JS：数组分块
来源：http://hz.gogol.net.cn/gtgtadqdpb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuanzx.com/gtkkqjeglr.html

[U111] JS：对象转 Map
来源：http://hz.shangyingyoupin.top/gtxactbusq.html

new Map(Object.entries(obj))
来源：http://hz.zhongyouzk.top/gtgdnddvon.html

[U112] JS：字符串补位
来源：http://hz.hnxiangtu.top/gtouscxgyp.html

"7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtqlnwcyph.html

[U113] JS：正则替换全部
来源：http://hz.pycfn.com/gtoxzbhgpb.html

s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtivknbqhy.html

[U114] JS：JSON 深比较
来源：http://hz.cucudq.cn/gtylsirmcs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtmiqpawgo.html

[U115] JS：生成 UUID
来源：http://hz.aizwys.cn/gtdgaogejy.html

crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtrpehyjxn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhengqikj.top/gtzlthbeod.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydjk.org.cn/gtsfvtfunx.html

[U117] JS：单元测试
来源：http://hz.316326.xyz/gtxhyqcvkk.html

npm i -D vitest;  npx vitest
来源：http://hz.jianghu66.top/gttjyenlgg.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gttftjuamu.html

npm i -D vite;  npx vite
来源：http://hz.guowangkeji.top/gtouievuzj.html

[U119] JS：生产构建
来源：http://hz.yanxiufei.cn/gtziutnpri.html

npx vite build
来源：http://hz.zhaomingkeji.xyz/gtvkvsfeee.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.wangdashe.top/gtxaalibky.html

import.meta.env.VITE_API_URL
来源：http://hz.gaohongyu789.top/gtzkipnocf.html

================================================================================
来源：http://hz.hywenlv.cn/gtggzgylvz.html

统计汇总
来源：http://hz.jinqigufen.top/gtpqigmsjh.html

================================================================================
来源：http://hz.52xcode.cn/gtzgzzqrtm.html

按语言统计（条）：
来源：http://hz.yongpay.top/gtazeftyoh.html

Python ......... 252
来源：http://hz.havefunace.top/gtyqmqbnus.html

PHP ............ 252
来源：http://hz.gotoacloud.top/gtmfqhbvtu.html

JavaScript ..... 252
来源：http://hz.sxryk.cn/gtxlzdzglg.html

TypeScript ..... 212
来源：http://hz.zhijiandao.cn/gtnirkwsuo.html

Java ........... 212
来源：http://hz.aizwys.cn/gtmwzcmgue.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtuafqukot.html

Ruby ........... 212
来源：http://hz.andypj.xyz/gtldprusjx.html

C# ............. 212
来源：http://hz.xuanzx.com/gtucnimmhl.html

C .............. 30
来源：http://hz.hammf.cn/gtvmsddflf.html

C++ ............ 30
来源：http://hz.hnxiangtu.top/gtqwupchjx.html

SQL ............ 90
来源：http://hz.fzhhl.top/gtrbqmjdni.html

Bash ........... 80
来源：http://hz.zhixingplan.top/gtezdfdtyp.html

Kotlin ......... 15
来源：http://hz.yj20258.top/gtbleejmoi.html

Swift .......... 15
来源：http://hz.yvedp.cn/gtqtdfigmq.html

Lua ............ 10
来源：http://hz.yongpay.top/gtqiukkfwe.html

Perl ........... 10
来源：http://hz.ppjwa.cn/gthhqdltle.html

Scala .......... 10
来源：http://hz.birdmap.top/gtmzzhhttw.html

------------------------------------
来源：http://hz.c1oappe.top/gtqogbierd.html

合计 ........... 2106 条
来源：http://hz.jiagoushi.top/gtjilsehri.html

按章节统计：
来源：http://hz.hammf.cn/gtzpkkwcvh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gtpzfrvdss.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtnfcpoeqt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtckcpbedh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtgmqcfvbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dianchejie.cn/gthqqobkjb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cashguo.top/gtpnxwcznc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtqxrbswss.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtjvdpbrcs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtsglwxlzo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.iojbl.cn/gtdpdevtyp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtcympktuo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtbbjhwevk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtwufclfvs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.pycfn.com/gtpbzssioj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.ybcxt.top/gtjipcfgiu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtrllezoet.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gttvtxjiqh.html

R Bash 专题                             80
来源：http://hz.shanyushiyangkeji.top/gtrgyccadt.html

S C / C++ 专题                          60
来源：http://hz.0kj1m.cn/gtczzufwcy.html

T 其他语言补充                          60
来源：http://hz.sysykeji.top/gtrekxzzxv.html

U 高频实用片段                         120
来源：http://hz.ydjk.org.cn/gtxycxwrmt.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtffxhcnfj.html

合计                                  2106 条
来源：http://hz.zdqjudy.top/gtuqfwgqsi.html

--------------------------------------------------------------------------------
来源：http://hz.ppjwa.cn/gtbpkwgbot.html

使用提醒
来源：http://hz.tianlin.xyz/gtcptjaxun.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gttnudwnvk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ybcxt.top/gtjbvayckx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yueranfly.top/gtzerqvpdp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hysaishi.cn/gtytwfuvsu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtgnadrban.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.haohaochexian.top/gtqvlpekji.html

—— 文件结束 ——
来源：http://hz.tanke756.top/gtseuwklym.html

================================================================================
来源：http://hz.jianghu66.top/gtgluqvvca.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtbqmaaxqi.html

Common Programming Examples Cheat Book
来源：http://hz.jinghuilouyu.cn/gtidgzcdha.html

================================================================================
来源：http://hz.hnqzz.top/gtrgehufhz.html

【收录内容】
来源：http://hz.kuanghao11.cn/gtjjjdryzj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtteclmiyu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gtbxfblbkf.html

SQL · Bash · C · C++
来源：http://hz.fzhhl.top/gtxhyrfzja.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sysykeji.top/gtbvokmmje.html

【使用说明】
来源：http://hz.yangfankeji.com/gtksroscll.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yvedp.cn/gtahmgjxkw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daria6918.cn/gtrrdpipye.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.meibo888.top/gtmszqkhrp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hfpthk.cn/gtnmbgmjum.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yonumen.top/gtglbkzkek.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sweek.top/gtlcvwettx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnxiangtu.top/gtlyhovwxf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.haohaochexian.top/gtfepuowgr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nwbrower.top/gtsxsixwnp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhixingplan.top/gtudslcxua.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgfzy.top/gtellaxpnd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daria6918.cn/gtnpzetiyc.html

【文件统计】
来源：http://hz.yj20258888.top/gtagkgirxu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.pengpengdd.cyou/gtzsoyijtn.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtkalcmbtc.html

目  录
来源：http://hz.sufxvd.cn/gthuuahfsj.html

--------------------------------------------------------------------------------
来源：http://hz.redwolf501.top/gtjvcjqckw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shzxlz.cn/gtyuoqbxwm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtjyetamyx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gthclctcts.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yanxiufei.cn/gtmwbamjyp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.haohaochexian.top/gtxatqryyk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zycfv.cn/gtmabwqarp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtzwpfbqun.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cucudq.cn/gtrbhgzwbh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtercnasqa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtwqllyvut.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aizwys.cn/gtditcabqe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtalgburwz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gttvedeiyh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.cqqwz.cn/gteobbotfn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.c1oappe.top/gtvqvxhmem.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtgcnoxftg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.aizwys.cn/gthixastsv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yj20258888.top/gtjdboixpa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ybcxt.top/gtsjdwilrq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtxrcccenz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinghuilouyu.cn/gtlcigtggq.html

================================================================================
来源：http://hz.sufxvd.cn/gtubcsccgf.html

A. 基础语法与类型
来源：http://hz.cheryme.top/gtjoxaeuwq.html

================================================================================
来源：http://hz.316326.xyz/gtwoyujzrq.html

[A01] Hello World
来源：http://hz.xuetiantiany.cn/gtaqlrvczl.html

Py:   print("Hello, World!")
来源：http://hz.zhijiandao.cn/gtebmhibvt.html

PHP:  echo "Hello, World!";
来源：http://hz.chenjidiqi.icu/gtsbxclyts.html

JS:   console.log("Hello, World!");
来源：http://hz.jqgufenzy.top/gtgnvsqnor.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jinqigfzy.top/gtjvbkrimu.html

Java: System.out.println("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtocsfwjit.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangshuangyany.cn/gtbgrzjbrw.html

Ruby: puts "Hello, World!"
来源：http://hz.tian-w.cn/gtzvvgrzei.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.fzhhl.top/gtswkkheve.html

[A02] 变量声明与赋值
来源：http://hz.xinyue.icu/gtqhohdirv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hnxiangtu.top/gtyciprfaj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuxming.cn/gtcaggtfet.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ybcxt.top/gtyrntptgj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.316326.xyz/gtexthirqf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gttxhjczrq.html

Go:   name := "Alex"; age := 20
来源：http://hz.zdqjudy.top/gtpkadfckt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.0kj1m.cn/gtbrnemsnt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.shzxlz.cn/gtrsdcapyj.html

[A03] 常量定义
来源：http://hz.gzhubu.top/gtyturgujw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yangfankeji.com/gtstvbzyjl.html

PHP:  const PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtrcyvmank.html

JS:   const PI = 3.14159;
来源：http://hz.zhengqikj.top/gtdoiivppm.html

TS:   const PI: number = 3.14159;
来源：http://hz.haohaochexian.top/gtuhwxjapg.html

Java: static final double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gthhtolnrd.html

Go:   const PI = 3.14159
来源：http://hz.daria6918.cn/gtgmgxrslw.html

Ruby: PI = 3.14159
来源：http://hz.xylfe.cn/gtvximkqzs.html

C#:   const double PI = 3.14159;
来源：http://hz.dashuyun.cn/gtwajxuact.html

[A04] 判断变量类型
来源：http://hz.jyoumei.cn/gtlnotxeox.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xylfe.cn/gtmgsmsqei.html


<!-- 参考信息 -->