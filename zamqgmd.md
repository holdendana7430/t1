代发 wailian999

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gizlesfjk.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gntzhzhdr.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gbrnpwjbn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gusvdzows.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gmthjrnig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gnpujywtz.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/glclwuyrj.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gytobzwwr.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gcpllbodm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gbcwjqkbd.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gojvzdqsh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gtwopxpsg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/grhusopjf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gclztnzbi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gwjrrusoh.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/grhpvrguk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gbypegmpp.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gnmvubxuw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gvvgmhrvm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gezhrfycu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gwfdohplg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gxiwzhrlw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gckbtojqg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gipdddgxr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gjsrjcsvy.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/grrhawtxn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gzygswywz.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gywzpfcmc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gtqbdydbh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gklxtvzhm.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gmcgurgkv.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gmenyzxkt.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gfolwknes.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gvkneqryr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/glsaazobz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gnufsjxsd.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gfqyfdtas.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gvqxwulun.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzjeuox.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gemucbosp.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gpsulghup.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gbpxtchjc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gepxvykpi.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/goacbohzb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/glnvmpqcm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gvpenbbdy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gslgycvbf.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gvhrimtsb.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gcttauqqu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gqajvrwty.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gdzecckue.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gnyfjmjlw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grobujuti.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gzarbxxgq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gvckufqua.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/guqzgmrmz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gwylbgnxg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gabshtcme.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gwtwbvhdn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gwdemsocn.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/giruklath.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gfpwaljkj.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gpgkazwbl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gogtbeagm.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gqukkowoa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gvmxlplbc.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gttqskoex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gxzndnfrp.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gaugzxljz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggpaxwgoj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gbfyetbob.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gttsbkfqs.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gaioptwwz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gxxapcoqk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/glxuvrxqn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gdqhvtdlp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gvijosxgf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gobvxeijr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggvlbhsim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/geyphkozw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gpkogqcec.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gnhvdmkdj.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/ghacysgcw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gqurabkcc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gronrxydk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxxwdhl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gecdrceyd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gnlntphzu.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gcprtngdq.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gxfmfbbqo.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gvxcgteze.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gyvcciebx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gskurnmgr.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gqqrsleik.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/geqqboxtx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/geyecltyb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gtgdpfcav.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gfevebztt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gedtqbnyh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gpbeqzdmu.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/guyppxtlo.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gctuuljam.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gceyflstr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gxseeyybg.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/guoosbkka.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gkjzqzupt.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/guesdlvqn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gfprvmmuw.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gztwgjmix.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gqgbexzxd.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gwjqvkutq.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gqhjnrcaz.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gkcivfdch.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gmwcwbbnw.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gaaqsiuxr.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gcjsromrz.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gtieoseff.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gthemxchm.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gxyunqczz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gluadwprs.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gcnkbwphc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/ggsobalnc.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/ghfwoqfft.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gttirulov.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gupbcdcgp.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gqzjuhczl.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gdjzfsbzg.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gursfdfxg.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gjqvknvmw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gpjfcqjly.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gulffqrse.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ghlizdhit.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/guetwzexm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gsbnwbegc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/goynqduhz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gejtxifee.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gaalkbkgj.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gosvcuwqc.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gcodcakpd.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gyzpbytxa.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gmvqdruvb.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gzevizdqw.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gyazfbsxs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gdbqvzexq.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/glhosijau.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gqcozarbg.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/ggqqaadlf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtkgvrdum.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/guarjpxre.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gkuqfmzts.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/grgtpuvmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gxgsgvdgg.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqiyfjgji.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gwerygmpu.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gokacqioo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gjsxbclsw.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gtgnrpqzb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/givzpjzbb.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gavcombxu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gifrzjvdq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/ghjjvacaa.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/ggnvfzvoq.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gqmkkpize.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjktejgey.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gmzvsqyga.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmcvbdxms.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gpxkujdtt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gawzjdrml.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/ggoqvrfwz.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmkbzafeo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gnbrbjylz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gblhmsylv.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gjchpzuwp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gzvbzeafz.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/ghkzfirdf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/ghhpurucn.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gfzypspct.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gpwepysfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gdybvaego.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/ginsbxdpq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gialrtxvv.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/ggrzskvvy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjcuxvbeb.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gjvmtbocm.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gawnucodj.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gbwxerhqn.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gksiglocb.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gzmgqdrgl.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gybauzovt.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/glwrqbayl.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gdxlxpdau.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ghqohvupr.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/ghdllhhgs.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/glxnstoqq.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/griqwsqlw.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gpnfzpdfi.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gfgzgxgvu.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gfarhihac.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gderquqya.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/ggurvyhec.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gwidzmuxd.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcjdukgyp.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gjvlqvefw.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gfhzyfrah.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gsdbgcjsd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqsvfxhcf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/goupvawhh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/glmwzpnmb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gytlszvlb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gpxbplkkj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/grqbkxobq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gqceloyao.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gkyrpyvrl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gqbfwufce.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbhvhrugm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gzglyeyyq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gbigxtjuk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/grhaknypj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gnkxbuvjg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtifqouwe.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gmfouvtcm.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gasalboiu.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gnsezeqke.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gnliocdyj.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gfgbuujno.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjfdcfmnh.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/giprgfsfh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gsjlagbss.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gjgpjmshu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggtjvjrvi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gvgypufay.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gwnvwvjwr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/ganbotqto.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/ghodhjbya.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gwwjyygnf.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gybixxaxx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjayhfdau.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlvepmd.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gwasszlxe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxckqffeh.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gwiwrpwmn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/guaumlpqd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/guwiruijb.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gthscmjcs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gusoszudu.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gvyrnbins.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gdpqveiff.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/grvmjwouq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gbksgfksf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gjabjrbiw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gxlytoeaf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/ggnkvtcxo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gdicahpjn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gllcjbzop.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gwscjrmsw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gcdeuwqlg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gfqazgltd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gcrgeasmb.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gvggcmtfx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gcyutduoo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gsegpqbbd.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gfhhdmpcd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gidjbjssi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gejvyplyx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gbrmmkfqp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gzlkcyexi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdifbcwfe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gtsdlctfh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gifwxwvxj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/geutttwgn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gaveqvzzb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gslzjxsmi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gkuzmburh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gwvbrccfn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/grssacayo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxyowjrzp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/geancziqj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/goxlairpg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gutsqnjpu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/getkbgals.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gncezynsc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/giykxpjmn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gflnusvhh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gdftahpop.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grpswtinw.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gwdawbenf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqgjmtxke.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gemljkhnd.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/ghnywottw.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gerwssncc.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkqwxpzbd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/grjkmbwgf.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gaoenykfh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gygcjuxid.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gxjunauaw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gprntipsw.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/goabpsrff.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gszonzejh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gcfzfgqcb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gnhfwmzdb.sHtML


<!-- 参考信息 -->