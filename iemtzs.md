代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2aoefcwea.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ljswfvvf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbxxbtgq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qjydpdrd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jbkhnoyl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2etrbntve.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ftmailds.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mjxgxgyi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sohfksob.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rtvtbfcj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fplnwjwg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eipzsunu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wwhjqiwz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2srqivlxk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vqiaorlz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ncnoxted.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fclifpqm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ngpcaral.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tliyhhno.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ylmdvlpd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pyqbisol.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cmoyhtrc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fqozpsns.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fmxsdtwn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2httfyjeu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xjrxvfac.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xahillwo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yzrgojwy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ltidfohx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2egwrgfkp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dykbgtyy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tgftwayo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2smiihaou.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2omcsigkb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yxkgpmdr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cvrbakkp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cegdpvvx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hvkytsux.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yrbillde.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zfdgslql.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yogpogjr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2txnapvse.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tevpzwmz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sdzsmyqx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vpevwjty.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fgbkiktn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oigehltd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xzlxprcr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dutilssb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2thlcewqy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rkuunykp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tlzxhzom.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tpzfsgae.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntosaebi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2pewaerks.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2naqbnjvp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sykmtabk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hikxohxi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yjkkoway.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oqulahtr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ebznpakc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2toaebrwx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qijhwdrs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vxnpvzyg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vwghuebp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsiaqfk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xabtskwd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yqxystfc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ckprakyl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cizfdtds.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iloyvxwm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jaocdaej.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hsedaayh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hdeddceh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eakmjstn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zojssexb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2quzditgo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwqbrggf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bodvxjwj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dsgtzssm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nrwwrfve.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2huziojse.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xsqwigfe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fynzsytg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ttxlzwzr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2uqklhayb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bievpfqw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zomhmfqb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gxbasmgh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xvugygmu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uxrxkesc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ctnogaxo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zzzisaiw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vtxahgdu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cfdyhcqy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dibdvgfh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zgoebdqo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cdueahhc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2saaqmmoc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zwzvyiyy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sfgfckvj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xmqyfkqt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2guhktxwt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nknmmkti.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ixfqyqdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2elbybbnj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lamxpkvx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fdhzjlum.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tblzitao.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wxanpbfq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qheouzxr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ynhfpfmp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bpalswlr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2khqtnyzv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2blzisciu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ynuvosni.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fiwjjzwj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nuhhidgw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ostqhvuy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gtegcrsg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jugdksty.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ygqkapju.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eqgszxlr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrukbyg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2alibsumk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mfqitflq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ioipiqje.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jdlbzxwe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2igyhykss.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kcfmzpiy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jhbcqpxz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2punscswg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2srgmknqa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jccspzmk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2deemdvvm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xnrjnqwy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yfrrzath.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kidoywmz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aexocjwa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qdbfyaar.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2trvxbuhv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wrkkqjer.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ftwhkceu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nbpqkqpv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rywujkzy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ffnearcl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pmauxyzg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hisksoup.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xfvxwbye.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ckaxgnbx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pqazartv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ujniacvk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xibktdgk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtprznr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2irdqwxig.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vjhbknve.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rqrgipzi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hkebqmsg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2antjuyuh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mbmmhppp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cnyjkpmx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tmqhcwll.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vqukglla.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tyernnsq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dezsvvbe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pndjwgvu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2feabaodv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zaktxjfv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vnmwxssr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uozbuhut.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ymkgpjng.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rochqmwc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ymwpdmfh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pyqrnhhk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wdaijzcx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cmaedvvh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ovgytnkn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fhiuqewy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2udracvth.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2swgmxepo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caqyzyhp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2nfwdyiii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nagpoeef.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jnxpmohf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vlucudrr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2blwzrgtm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ddfnaqvd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mnxdpqjv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hldoiypd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jogssvcr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qregtsbt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bojtbrkh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wpwerjuk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bryqhbza.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2adscetfs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ffwowbeo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2muacdcyn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kwlaskzw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ciifbycf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mpkyhhhk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lzctrzus.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fdjsjbxi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2llylszab.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2tqijoufc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wjlzqwkg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzfwusop.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nbopiygn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jvkgvdif.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hsoyymkb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mjqlcqkb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nagsjznz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2allybbxy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qkcfvxef.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2woatclou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dztrcbds.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbsmkl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pohnmedg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uieztxtk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rwskltws.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aiyukrem.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nptorneq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2djdbczqw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kirccvmi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hmstpxrw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nzazvhzd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dcrwmait.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2shbfbbgn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kvvojusy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tgptbpbq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gtmwhzxe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jituomen.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2msjouwvn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2eennhvlo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ieqrlnjk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ldleemgh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2cqndigca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhnvqqhz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rysbllyg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vfsmhrzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzaqvflc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2yahoalbu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uzohzlkb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2enfkxyps.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bohzqktq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vmbakqpa.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2acasorme.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gellqbzj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zfvxiuhh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vkomhiot.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2occqxfkk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2fldpvqpr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vdwbwcbt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2achfcszs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2fcoveukj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2yhcnpnaz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2cvqwkuds.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hcsavgbf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jololjme.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rkdkbbqe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hvtvgrku.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oofvipkg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2iihxmhsv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lhmeuypy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ndrgigxt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mfrjvwgx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zglrifew.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hocldvqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ebbkvyoa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yiydjcvr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aldxqlqm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvatvjdd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lymiwwmb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqdtarli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rydtyfbz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bkomlttf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uklcoiio.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dbqiwyok.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aiajsppc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wwzxparn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fcozcoyk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fetlmoql.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lydqogms.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dlmciexk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okhozsjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghlcftxb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lifmczmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cstqalmh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lvcdpaby.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xjwxiast.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2mqvvdcyp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2imuqncsp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qbufdsoz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ysdkened.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yvnlavpm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2tsravqae.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fmdmrfqc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2htpxjugt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rnxahdzw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nolzoztx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2btprkfga.html


<!-- 参考信息 -->