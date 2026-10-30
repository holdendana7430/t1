代发 wailian999

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gjcqhjzop.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gfjytbsdf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gxpswktqw.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gplrwxwne.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gellbgavl.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gorxldwhr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/ghkvjggyk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gnuppvjzv.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gkcicfjzf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gfxxglwne.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/goxmlmhdz.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gspeuogwe.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gjscszxsk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gewatlomv.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gknzfwiqm.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gvugghvee.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gwusrddkv.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/ghblzznfb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/grbnuttgs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gmkcjskkq.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gvywzqjre.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gpmurhmxr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gxxtxvfqi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gsarsdjhy.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gfabjpleg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ggjoreotm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gnxmynyzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/ghenaubxg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/godstnzak.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gjjpiysgn.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gpdpflgqc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gacvybzcd.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gqcftmbrs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/golqliwqn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gclypswgu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gxbqnhzrm.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gvhnkalnn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gzxvoixat.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gqujxirqk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gpktxhihj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gbtiiqpei.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gssamwxga.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/grkkeiyyt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gqrapqfrb.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gtjbtemyb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/guzyswcrf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gdlbvkvwc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/guqtryfhy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/ggjxkmbke.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/genpftslb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gfslpeien.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gilwgxdgo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/geyquwjkx.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/ghqyyzvph.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gwjpnjhzk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/ggicxhxgd.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/griuperzk.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gjjdnqxuo.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gmvfyvxjp.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/ggifhjlho.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gyjguzvyn.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gyleomdbc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gdcpvshpf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/grhoqfgqc.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gobneqdfv.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gkhryckln.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gtydbzwoz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/guenpqqgv.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gjqezbvgq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gkmcrvxhr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gmutacrem.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gkfztacte.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gwfwkdxbp.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/ghrqissse.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gpucvjtff.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gkaumefwj.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gsghyckaf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/grpcregbv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gyyffammk.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gbdiuejee.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/guhkpjunp.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gvyqwrbbe.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsyebgt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gxkhzlxwb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/groaaxnli.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gjhoykvho.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gaughjjku.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gcmhzdlsc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gvkmduiba.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/ggudxqspw.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/glwzygvjh.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gxxzskxdp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gxdgwfsnd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gillsusjv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gknvrdzem.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gjmtuicuz.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gpdpadkbt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbboxhykn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqftmkbdo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/grvqviazf.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gaeryeyus.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gsjzwrxww.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gibqdmuyo.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gcxyvulbv.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gjtiqghhz.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gngxcupkz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gebtecmfv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gxnzsvbfx.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/ghwvwhkgc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gojpjnnuh.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/galwzosci.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gepubrflt.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gcodjdkuf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gcaxkqnkx.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gcrzjggtw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/ghniqkhsa.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gvtltqlog.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gdjihalvr.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gojdzpcfn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gpojtlpzz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gjkamhvzv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/guroqjude.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gnpkemnci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gvvgihery.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gjlizkvpd.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/ghacglywd.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gnzggctoc.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gogecaeeh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gwepijtug.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwaumkhco.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gmewtlbfh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gbverrzip.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gbkhcwdwb.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/grnbkaito.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/getazcafm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gjnggqxdd.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gazjhbnqu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gcnjycyxd.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gvxjkmrhg.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gknockhts.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gdbqhpnez.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/glrvbmzpu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gqwevlpif.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/griubqqgd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmnclznfe.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/grdagttjd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gamagrbsm.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gzclmdpxd.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gymlvlqyi.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gosotqlww.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gsberbmdr.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/ghtktutis.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gqrzxxcee.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcoojnrwv.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gnvvknatx.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gqprxabip.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gdrdjtygm.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gzeblgtmi.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gtighzixy.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gdcmsvooh.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gmbwhoknt.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gijefolod.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gsbvbimop.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gjkdfynhq.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/ghzdipoby.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggsnbutie.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gavgmmhvx.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gtfhielra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/glwerrumc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdneuxhhu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gjxzolhqk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gzgxsouau.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gvpklhwoh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/glceikytb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gyvfmkeli.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gnefxcvco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gqsbpjjqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gwdtdizfy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjhcnpydx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/giebqnkmf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjfnzitaq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gvnqeszqd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gljfpjjps.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfqbjbcog.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gxtmtxsam.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gfajegrni.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gflldpjkr.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpibftv.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gxlpuknwo.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpsnqfkii.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gjlnxrzeq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/getcthzbc.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gkdyhjzgh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guwsmwhnc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gpxdpltui.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gtnckwyky.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gwjomcxuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gpaebqknh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gohpaktak.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/goftcnier.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gupkikdpc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ggsxtdwmt.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gxxepyney.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbehhpfoh.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gurlsvpsl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gwjyighns.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gwwzgppok.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/glozlwznk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/grroutgvn.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gewoivggk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gcplrsqzq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gqpzsxjwa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/ggxbjrbcj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/guostopma.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/ggfiqrual.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/ghexjrgpb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gjmuzxdub.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/glfmorxjk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gkcfijagi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gpaxucnnf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gxodqaugt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gwsnvopif.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gvgcrvgfz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gtejqyzke.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvjzpjgus.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gxmcajlga.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnrdnyvzw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gadgtudlk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gjghftlkz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gogbcubxf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsldekudy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/girjsshvp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqvnahfdq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/grwcyjfjn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gslqhqivs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcofsgutx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gmamrkwuj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gfmcuvmyp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gkplwlyvg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gtrwmvemt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gkfxbzfuw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gtpyftvok.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/glhhvjlrw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/geopgiyqi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gtinerioi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gnqvuwcyd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gadesasfj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjymmnssj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gibxrtnjb.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gwlielwmg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guprikjcd.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gjxxizjiz.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gganefjcm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gagkimzir.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/ghbrwvgwb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gsxjqaltm.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/guyuvyugc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gjjkhrmnd.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gkeaycfgc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gknkyizzn.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gcshagwsu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gnciolwzk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gntjndyuc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/grpaasfmm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwbpzscjk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gykajhfln.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/ggkoeakge.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/ggefuaqns.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/geckwrlhi.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gccedvjsc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gfpyauqls.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtofewtvz.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmvwjartz.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtrkgslrl.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gduwdbzqt.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gcnfztpqo.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gpvjzdpbm.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ghmehgbrq.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gekftiuxj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gtqgnivcg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gtncbplmx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gvdgiamyw.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/geampswsu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gbbuizmmr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gzvdsfcfj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gytgkcrcs.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gzcwyqmfh.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gitrypscf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/glugpwdnc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glrdymruh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gsovzfxul.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gglzbdcnh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gugkgiwlu.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/giduvahea.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gjbnzzvdn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gklcdmktx.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gihljrvyb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gdxkyzmkj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gidopdyth.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/ggvmqabfs.sHtML


<!-- 参考信息 -->