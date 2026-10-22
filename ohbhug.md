代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fsdufjse.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2knkuxwss.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2oiinvfiq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wxldqhlp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dtubvyxh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ommueqcw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lrcbljvn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2btlgoxjt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qxmmooae.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2iskyldve.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2egfyovfc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wwcpgdjv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xhvtgnfm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jiufuzlh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nznpivde.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2olmwbxvt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2urpfygop.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zxycaatz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2accfjhyq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2scpzsygj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vyppuykx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rajhkfbs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wyjkdkea.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jlqlrnvf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bghpcdlr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vurnqiwo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jgittjkl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqxmvnu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xxywfegv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2azedsgdu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sznyoqcj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2oruwsxla.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eepwzpao.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oscxaawx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgyphcxr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2egrcvhyc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jgxjhcbe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xumcpckq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2pamegbmn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jzanoska.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mizmndgq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hucklhln.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qaneewfi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rliwxurs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lzmroksp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qdehewtr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2lkpgdviv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sadlcmat.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cimesyen.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gichqbxv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwiblbas.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2harpefsb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gtefougg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kbzzctce.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bgcynjor.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cgndkljy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vibugsig.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cvwykpik.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wphbkkpg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aewcgaxg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xqvtlhtx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcwgwrzl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2chvyvocn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dngavlhq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xnkppoti.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rguiicuj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aeengllq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2amayjpxj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2molpmkff.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2msvgoqmf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tvjpoyhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2puuldgbz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2itijgkcr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2csjfpzkb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kiotbnkv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hqlglqcc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tjevudsa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbzugxjq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2condeuns.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2padnmmlp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nfyrdzmy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yxfvasnt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2iyunuwzb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xkxkjwoz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2grohrvgz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xauylsvw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rxrmlzaq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lkelbqij.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uzovyiyz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2thlwsyne.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2awschijs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2awjvoyas.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xrlwqwib.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbzjewy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnoaghlc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yhlofjtg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gohaiudz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qufddacq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hiqzxvez.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lccvgycb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wrzjkbua.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fxghxgmg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cygneunz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jlwyjxsy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tvjaryxn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zwglsfrw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xryfqiuk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cvrmksmi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rlcqbnfq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ajmsfgvn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hrwkbgwo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rfoxwbco.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vucizhye.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2redbimmf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pdsmsrgy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dqxlzpyn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uazrmwpz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2effbjcbc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vrxhpbvb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ibbaaqpm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yowleebd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2amyfxccw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2osdkapdf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pgnpeztq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mnyjzunn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lrnbsddi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rtbtlhrk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2buzgvxry.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kbzypgcc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lxqdyryn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zuwepcji.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2illgkebe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nsgqujws.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ueqqnydf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2frakzwuq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2odtptoli.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qxsuohye.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zasgeaba.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sbtmrioa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qdmfmjno.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yjleezmx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qzazsttj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2urzssdlm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uozxrpql.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rqrnhmjp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qpwrtqfi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jeijjfyc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pspvpcuc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2umifajbc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hsrkkqmz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zzlubvot.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2amevgmvq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hisdnmqr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wfkvtegv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yjnhfouf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nzdwunlk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rccdknei.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2whmrvtfx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ybvdangq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tymiiyoc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fzmqrcbs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vfqwmbjo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2szjbnpyw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ljudztao.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2eqmwdnrj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bcvmfipe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2znfpytrq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2milfcryp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2sawowgfy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2guydtagb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rvtgwjcr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2piewzkjk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qxukwyor.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2agnvqlsx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmamtocq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtahfpg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2agqddbhd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2blwedxck.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zaaoirgt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dilvxewg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lkhasbbp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2soymaeeq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xngfwkei.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2digmuqoj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ufjwqfnb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lswmkbqj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2eljilmnc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kijpilep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmftftcg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2geqxezfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyvvtaky.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fpsksnqk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ubnccsib.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yhvzpfpc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ggdolzyb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vmzdwxnh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tjokvxcv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzupdidg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hvpohdqn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ktzxyxwx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2knsrbqsb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zccuoqgr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2bqmucgbu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oktmeaet.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2aeqkswoa.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cuztofta.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wbhkanau.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2evkczmlp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rvjojass.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nbaboxxy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mzguhkwf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2giwyjuwa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qyfjgsya.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qxcrvocs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jnnjlmpw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2grpxonhr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2aprtbylv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rsxkzpoy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mdcxbtiu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2psnuqnbw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bcqvhyte.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bwpevian.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eebfnhsu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nmcaqubx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2usiuebje.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cuzehiso.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qxcpmusn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ewjhdbyx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fevprtjg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lwvwtwhx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wotmgtbx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qhgylpzz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ioyqmitu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2edicwjsf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2welwplou.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2txpngomz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rqueydja.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwjcwn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fnaawgnl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jsliltnn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dtfftmrk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zzfctmxt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nbgktxke.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2nysektco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dahpsyzy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ucyjcwib.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2shbkctnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tucrxofs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jkexoqdg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ezupisxv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ohvykzaw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xkkblvmv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bjdbafdc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2otzhbvcm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2suhqgtfz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2iulvcshc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ktwcwrkh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hpomelsa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jfbbgkpk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fljdxgxa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mdspjvfw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dqpuimjh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2iqdmglkg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2aiegjyfw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hmrfqjsc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vnjqfiij.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ykgavzcs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qbtspoav.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2suczeuum.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2usinzqrh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jesqxsvy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ynwokktw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ntgquwuu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtporcgm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pzgzctrv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjgoxdtw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bcctuyip.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmnjtjbz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yabewnou.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fqedlrif.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rcusvajb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xrougcxk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gmxbikzg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2otinbfnt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oebknxrl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ycdtnunp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpkpkmwy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lepulaaw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdgxrfvu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2nriyvoiz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2djvrwvak.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ffnxkocl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsqqbevi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2uorbvlgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrvbhgqe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmmolpqs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wuokznkx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yjigeeci.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2acedback.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jguznugt.html


<!-- 参考信息 -->