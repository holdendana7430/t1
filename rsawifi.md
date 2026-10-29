代发 wailian999

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/ggyyqzaud.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gckaulnzn.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/glzlltqrw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gusrwrsuw.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gduhhheef.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/geprkcrcs.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gkbdutyqr.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gtbfqktyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/ghdzccewh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gbswlveec.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/ggidocvrs.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gpcrgcrui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gabsjsmjq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/glhnccxyr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/ghzrvvzxf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gfurkajjf.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxwhexdpt.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/glcmutlyg.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gtivomzgo.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gyojgwulz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gtagypbtr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gwnjlfiyg.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gtaythmer.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gwnrrraat.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gcdhgspdv.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/grtosdytu.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gdhylenvk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gzawksglt.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gqddghrri.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gkleoorld.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gqsmlttgr.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/grhvoqzas.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gimsyocfj.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gcqqgfxeh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gbxujlhbx.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gazvghfcc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gffjtbjmi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gsldptiod.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gmdhfzjym.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gcidtmesj.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gqdwvxfom.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gshfscuht.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gsigazjcy.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gjsitqscf.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/grqxgkdwc.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gqgjfgppg.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gxascrozl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gahkquici.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gvyiffher.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gyahbomna.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gepwqukpn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gvddwvuql.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gbfdwwdnh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gynjywqoz.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gobhckwqi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gswuaxkdj.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gslnluehh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gperdiswk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkwzxggsm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/ghvwbbsrj.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/ggemzdejc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpbnrubfb.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gwhfotxpd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/goqrlaooe.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gdtkrccww.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gtorsjoeo.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gtjinzgyo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gxwqdpmbr.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gaxbfgxqu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gswurdawg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggspnzedv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gcpxybjct.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/girnqtbwz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gukcqfgtz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gsmjulrjy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/glcuzbzmj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gjwijzfow.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gsuchgzyn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gwhnznyjf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gyibzelgl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gcgruwhkg.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gobzikfcy.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gtqzfgbqp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gsxeewkld.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gzyjuhvkr.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ghkgcsnzk.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gasnxfafb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/ggazbqwrs.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/ggvhtrwon.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gqqteodjx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gqzimmasj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gttzqteno.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gibokjmqj.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gbgkhztzw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gcixysmvy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gkkpjkios.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/geytqwepx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/govqabihf.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gobmhtuhy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gzbtrvyxa.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gveodcdzn.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/goxqbfaog.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gctqarduu.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gbwyakail.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/ggrxzozxd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gsnsgjojf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/ggeocpndz.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gzrysaxpu.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/ghhuvrbup.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gljiqupsn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gbavggfsa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwhybkvxt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gaccqurvr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gdiesgsbk.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqnpplhsk.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfuprsqmo.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gmveuviuh.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gnrtpumme.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gyefmhams.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gnuqocbmd.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/grrpbpzly.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gkbkcactu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gtcfojfzn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkncklplv.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gwdxnehcg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gfuvftghb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gvzdyznrd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gfskitqlv.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/glmpuytrl.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gkophohfx.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gywvsoiqf.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gbgsstude.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gndgfuseu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gzxsthnep.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gjczacmle.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gtcunnnyo.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gbyqybvpf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gywdsxdhz.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gqfhkshhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gckoqjdga.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gkwetrcsd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/goqysyhdb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gawjsrgib.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/guhesqrpa.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gjgmovwat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gbwrijrge.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gjmsctdxl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gjvizwjnm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gwwgbrrcp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gscajtklc.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gutbjsrsf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gpxpvefko.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gycrenrgf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/glvcqdjey.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gcqchujhb.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtypgiudy.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gemgxjjdd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpcsllebg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/giqhpfdbn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdlceqxrj.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gxfdvsrtc.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/giiebkuvj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gvqtszsfg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gxpfgxlgb.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/ggardjlqn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gtgsagezh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gpptnpptr.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gcccfcgvi.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gvdcxpzls.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gzklbsyme.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gacojvgtr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/goydlunja.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gubcmgjpa.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/ggkdodzrz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxarbtffc.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gccxvljph.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/giqwskobx.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gcrwkvlql.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gmrghwzkw.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gryyofyuf.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gkqqmfmeg.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ggdzmhbpo.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gxrqudhnk.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gqcejkwts.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gbtutmlft.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/ggavlacbu.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gnnqxdfzh.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/geldtsanp.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/ggedjnkjh.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gxchmwxcc.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gjwbesefa.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gbidinptd.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gyytmjgks.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gyltmumch.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gqjuffcnf.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gdxaqddhn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gxrfkrrjl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grmcnqwhs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gdvvttucm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gceilblxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/glkbchyoh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gcxrivunm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gctcopzyf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkthahp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwuvmptoe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gnnfsyojo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbuycncrf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gktxbmwma.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnsgdgtda.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/geowqypql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gbihsbzuw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gdduqbhhv.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gnxvmjncu.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gelcvkmnu.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gqfmjajus.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gbhbrrfdf.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gpdakquiq.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/guzrvbobz.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/grshcxlev.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/ghurigmhq.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gohmbibza.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gzejtonht.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/guztsjxpx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gqljmszho.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gsmosbdeq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gfgwfqqgg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/glohwviax.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gcxhofajw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giwywvqeq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gkbxhvoxr.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gwypokkxp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzohvgjyn.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gdxhnqiqw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/glujhtxds.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/goxihdmfi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gslkpbbiw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gtzojvtpy.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gonresbac.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/guzslkpvh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gktmiynhi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/grnvqovxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gnelvddag.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gqxcgeszk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gejxuzayq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gkolgasgc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gxangeevb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gcyoyzprz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/glchfjthv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/ggjghusiv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gkhidderd.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gumanztdk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/grtzkrexp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggqpxrhsv.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gwbrcexna.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gozdqddtu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gtvxjszzd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gfbjoelnu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gnshcvxid.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/ghctsocyx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqxpvvrix.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gwrhalxov.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gifrizxst.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gkuillyjr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gtadcfjcw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gimsbicaw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gwrknvywc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gbsiscsak.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gheeetkrv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gkridawpj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnxsrolko.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gwxjkqcie.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/ggjzmegrz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/glwybytlt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gpqmhpsfg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gwqzyzzgl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gkutfcfuw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtdblrnlm.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gvhwtfqnl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giyxhhbgr.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gaqmeacwv.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/ggtpdsxdl.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gkckppahl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gvhfojiok.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gzdbomllk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/guorbriff.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gnbbaokvm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gyvuarbum.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gnnhfdwkz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gunjqmmtp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/giuaozpab.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkswiflcm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gevlyykma.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gqqkiucdn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwgyajstx.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gbpysnbtz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gpkucoope.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/ghrzfxezt.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gxjdzlcqy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gtaoslnwe.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/geicxdkup.sHtML


<!-- 参考信息 -->