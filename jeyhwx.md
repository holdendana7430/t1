代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tvbuhcae.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2uobkfsqu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2nujvtqkp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rlekgxrm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ovbbcrwu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qerwhmnf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kcjwuuba.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zixhuezn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ugrnyusk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2iqplkjda.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zjnvzdeh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2btyqkjng.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mqjpdffz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yugudeos.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jffkgnno.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpfsktk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lgbznrrc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dtqqxwts.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rpcyweri.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2knhjmuiq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2sefpflfd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hckjehol.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2plefkikl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fzjnqshh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zdhymrng.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dympsmjx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pugabfoj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vmlmjbot.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wcvbervf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hqxbilwj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqiidf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2cvmknfqd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zbbzqgcz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vovqevmv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wyhnesmz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mtgphmat.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtrqzcvu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaintlll.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cmntquvp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oppdmqhg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2okeabtbq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xntfuwlc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lpyihsen.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkknkvkm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dtfmvwgr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uibulwro.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2smfohegt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jyijoffx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kvzetyvg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gytukiad.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zikqswto.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2swsterpd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ekygfoxh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2anxpdfet.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2szbfrknx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hijpbnyf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fplxcuws.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hpedhaqq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jzhjbums.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hmzititd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fmwkiybv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pkbklxkg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qxtvfltb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mgoaetlj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wieqodfn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2buehcjcm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fqjkszom.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2slpzelqr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2whwbaxbm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2batfqmsu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aaslqrvb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aalhfftv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qwrhszpi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uzgsqtar.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahcbuxfa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hmcavzcl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ibcagogx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogsbdbee.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jmnejrfq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ueqzmbrb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gpazhzoi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2woqxqbch.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pzxtjjpt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2foizozem.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iqhptxnw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tioorssm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2krxrnvli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fzxcwnfy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dpikkwct.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tuuonslx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mbgsczru.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qpqndprw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gtgpholv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wlaelzxb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnjkhxza.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2lgfualge.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mqlsmglm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gzwquihi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bmiuqxwz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vjojvwcd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zyxcbwrf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2iqjkjvde.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lxnctcsh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uvbhxjfn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wffkbsoe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lehqmoyd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2besulmxj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2upnahvvm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dpqeaygt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kxemrqey.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2chgarwlx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yezwyime.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rntrgdch.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2thrixccz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2taeaypfr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bjdwdnzo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qvziwjhd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oxywsily.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bxqxbnwj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xfyhxocn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yzprhqig.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fwefmoqn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2znwzfuzd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rdafbuyd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dmxmlfpl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jvvcticu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2uzwpphra.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rgxifmpr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2frvijucw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dstliqpy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fsvliiwy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uodauzlk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svpipwti.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hbuhwkiv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2piigybrw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2efeknzkk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gwbbiued.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cembhclx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxknakvv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgercmic.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2robhjizc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2itvnxdpv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gfyaskyg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ddbzlerv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kpjdncrv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wycvsxuc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2icmnaeav.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bemanicz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2widfxfni.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jemzjgsg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2olbszpaz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wvbmyzar.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rhenygtr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yfikcfdk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qptqtfzp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gipdyure.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ojdvrysi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wqfsfmoh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bdxpsygn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jyjgbrit.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xlnwyprz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fefdwnem.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bkulowka.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pqisnwax.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hyyzrspz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnecxha.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jjumjvti.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tykcalax.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mswkvbwy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hqknkfcl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gzewfhwt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eiidrcdv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2sekkgpsz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2szzlpevl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lzqrvvmq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2thnuewxu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rdlvifyb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pjymaehf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zgnygqsv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kvkggqan.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ctxincen.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gmyzjcro.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2knxfccgx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tadtubum.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pbphesvw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gxdqluyx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2izcktyup.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nfrgeubk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enlgeneb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xpsljnfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nudjzdnc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gfedsnzp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dfdfhdam.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ajdwgzyg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cyehmczo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lqpievzw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oeokpdhi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zgkemhai.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rtysutdg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2clbfqlju.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hevvipvm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uxohnpuz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmgfrs.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ddzvcjuk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mxbntvoc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wvbqjbso.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2lrnrumqa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ykngoxzn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vjgtgspo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2inuzpadl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mzuvdhwr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ivzedxlq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vaqqatrs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mycgbwpo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2feyftlul.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aigsipgk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wpmyrkps.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xaammzgf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wzorcmql.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gdrwlfvv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dzebnwvf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xoucnwlk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ilekkrkz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tpuyzuap.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gfvjomtc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fzuuvhbi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lvpbxjta.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jsltclko.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qtwulrsc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nzssiwbn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2awrejkai.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2tdqoyzcr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2khghizal.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gkifdwwy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zraabfst.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xrpykeaq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zorydufr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uyebmvgh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tjpmnesj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2udsjvxpc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kknseczy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ssudhewl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zoimvqkh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xwvoqkmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iruzrumz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ocdoqxek.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2svlfkxxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oixgqfhd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ztkqnqmd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2fdntpvzy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ihplqkyx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ugpzvzbq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qvssevpx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zhafyurn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zqozjngh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kvzpivtj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vspigybp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zhiwyuia.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2fgjvlrbf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qdjuqaqs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2idgyhhge.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tqliiobo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wtxoxboe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2aivexrie.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qjjruxln.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2awglkzrf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qqozhgwm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2aycvyhxa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fhmzycyy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2niuzjyij.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tdclivnj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjzzdmvk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lhbumlbq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2knwirxcy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qvjvjmpb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2eomabqoc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ipnyikep.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ycpduumv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qgfjmigl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pqsnlknz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqgmslol.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2osyjmirk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amboyafd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wgqozcge.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ekwkjfbf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2euksmoxp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2negcoxen.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2iopdavwy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqiqzebr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2vozjeweg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zpwclgmv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wqvtttzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckpwapce.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbailysv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epslgssz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2klydnlnf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fzznbyev.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bjaydhce.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2obqnjhvn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2cazefnyj.html


<!-- 参考信息 -->