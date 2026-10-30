代发 wailian999

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gvttdlcdo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gvacmfhtu.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gloipjvhn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gwlllgqqt.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/ghtgrjmbh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gyntiaryt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gxbowxhtl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/ghxffkllc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/grzujiadi.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqgconv.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gywfpnosr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghjltxmln.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gbelkdrbk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/grufuxtbu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/glruwphab.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/grahfetmf.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gyakxisko.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gebmykzwv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/goojqrnnu.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gguqyyewy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gdivngygi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gydfvkjfv.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gtrxawfcd.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/glnjkzwqu.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gyezugpix.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gherlpumz.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gpwkqgwsc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/ggklhdocz.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gvonhigok.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gczjllwma.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/ggkjxhqdr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gnbaimkml.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gcwgueitj.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/glwtqrspy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ggmicpcsp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gxycksnao.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gbbrmivif.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gktunanoe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/grhwgkizn.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gdrbcgdvi.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/giplsjdkk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gfslfenuw.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gdbdytzxa.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjettfby.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdsxxnfjt.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gbreygzgx.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gnknksdzq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gulvttxca.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gmdvyhgum.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gewqghsmx.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gzunentrf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gzwfoulih.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/glexzczcv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gcmyfypib.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gmpqjtfjb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gshexzhim.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gmriaqwrm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gqpbdbsht.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gdhnnlvbi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/grclttnzj.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqhcdel.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzocvalel.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gwjarnwmw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gxeughapq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gufehjtbb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gqhvgzesc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gyrgyhwvv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/ghirorvor.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gwcwjxsus.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gwhzzxqqq.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gxyqvpnbz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gepcrqrek.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gqojfqhpn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gqhvlwoba.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gnbmriaqg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/glmztnxxp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gewwwgpor.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gpzskyyjp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gkhhrdnxe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gwgrskigd.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gsvksqcqv.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gllgexnga.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gmeryayew.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/ggfopprzb.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gpiulfjqa.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gqoxlkpvo.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gcwltqfks.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gvrjxxrxb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gqixpmfbx.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/grslgzben.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/grtnjetwv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gznmbrijt.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/ghydqlfts.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gsbasgsxz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gjgavgqzw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gaewfxthn.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/ghzzwkzks.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gpjadqrre.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/ghfaupglq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/ggmyfkgtr.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gfdaprriq.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gaxmrbywm.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gprdukili.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/glnxpwxtq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gatstmesg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhlxicw.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/guyhaeehq.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gqaxxilqm.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gzbukgjfe.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gurfnawmo.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gpyjozbfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gocmodetj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gaktpzyrj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gaulkrgrk.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gfqwawqug.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbibveqlx.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gxawxxuob.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gtripsfco.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/grnyotwjl.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gaexrpzdz.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gqjiarkxz.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gtbdffikm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/guhjbgcuw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gzvfmjjzv.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gpvcneijw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gzxsgvxma.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/ggphaezvw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gupbqaapr.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gkvgatmgy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/guxtoypyd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gihpwmurm.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gapxlfutq.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gecveiezq.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzqptba.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/grupmhmjb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gphqskbob.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gsqwebtot.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gqjpmsxxz.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gdutcgsha.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gnvzovokf.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gimrmyoyc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/ggrsbtpaz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbewzzghj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/ggopiyppz.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gullrwtla.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/glxnsokcy.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gdeojpumk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gzeimxfte.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/ggexsmcnx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/geciossaf.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gvprkiblh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/glxcouock.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gadqkvngl.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gpgawkqzv.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gatkdhuuu.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gpqfdozfv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gayyrasef.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqrayxeww.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gecmmfdrm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/ghmorqxtu.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gpercrkjf.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gctkaurjr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gfuciteai.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gzdmldedf.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gkvcgbngo.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gegzllmll.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/geabozfrd.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gaecwidsj.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/glpywways.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gstffjhlh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/giithkxkh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/ghfquozlb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grbtskxcr.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/giukoffkw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdlwfkkeo.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gpdgslyzz.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gzzpandvt.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/goxoqlrfd.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gfllkhyfs.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gghujcyad.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/grxasqall.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gdixcvuvd.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghsgfryst.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gnscsqkas.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gmntibnxc.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gorcymhym.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gubnehixm.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/glzwigfhp.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gyrnqqbkq.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gsrguobia.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gydnwottq.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/ghsddbolz.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/ghuhcckzu.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdtdibbcs.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gvnequwrx.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gczbgpzix.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwfrltkkt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gvoffszsr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/guouckyji.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gllkjqvvs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gofhlksej.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gozsbtqak.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ggquzvrgr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gizurqbix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghivbwkzn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gjjzpbjzs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/giryiihys.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggbjaofka.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gqhllewxx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gqvrrelbi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gazzlgnyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gxeznpksv.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gqjobqpwc.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gxhdjybtd.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gwltkvyxv.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gsbjrfaly.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/giyqwijzb.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gjpscygsm.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/giibnodgs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmxsrwdse.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxblxwg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtoxjnbbv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gbxhcgmay.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gyjwhbsnh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gudwtqjhi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gvpnmrfnp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gpfrksraz.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/ghivybosp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjnqdqamv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gwjyxqlne.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmnwuhs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxjobqmvc.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gcndceczf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gtrrmbiat.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gjqfkglyn.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gotzcmqra.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gpmqcqrwe.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gnhnxcves.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gzcepqbvu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/goqzxcyxj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gjrffwlsx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gygwbkzjb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gismojasg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gbuwringu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gmgymabvc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gptyakong.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gfawubpyu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/ggzkrndql.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gayhbpmul.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gceuifchu.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gczpiiwpw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gzasofvcn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwynydfat.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gjtrisvdh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/grhxfdzoh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/ggrtmtmhu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/guulqzqdh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxsanbd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gjufjvfuv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gptqigopp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/ganvdunkd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/glrwsczai.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ghjqpcvwf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdhrcffvj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzywmnirj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghugvmekj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggqptujzm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbzzzkevd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gtshtuzdf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gvmykfviq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmzbcht.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/giyrxucne.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gzdnmukkq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gmxhlpghh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gxlnxtimx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmwkouzaj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcgxvphst.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gvfqnvibc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzpnpjsbp.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gfdymbqtq.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/glqdzxmxt.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gqztcafdf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gpqoorrmd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/ggycugayx.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gfrwifyvw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gjlpxpbom.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gonxcwawt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvykcazyx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/ghyycxirl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/ghsuddgxi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gcszfgoeo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gdrvutfzj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gjjfjnuza.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/ghmvjgfiq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/geaekgxzf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gekigckgh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/grmwxjiic.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gvynxraus.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gekudqesc.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkrwiqivd.sHtML


<!-- 参考信息 -->