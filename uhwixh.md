代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jpzoofrm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rrqnsabc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zigjxhki.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sttdjrlw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dnowrcsj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nizwoxfq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xoksznoh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mdwlcdou.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qlbbptmd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rxiycsdm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2djlyylsx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ackwieux.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2aldjmbst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2whckpmyf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xgnrkfso.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dxlbzkdy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ehbuwkwj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yuraycyf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ouvpctzt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ilwsdbdq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2krmkjysy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mwvszcjz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nvreivse.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tetqivfk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lszblaqk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jykekdut.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kihcbqrr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2chegiwtu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sqomgxxv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xwapjyft.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vagalmtc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rkgfnoyh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pibpbjhu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jggolavw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mvhomznq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bgvjzpvt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmmydght.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhfljho.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2idrdfxef.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fqlaudod.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zfwdninh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bkqbrzmd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wpmgtkkj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gecjgdci.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fetshkyh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mphzebxb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2oelhcpds.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqmpnewr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2feabqdkn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jexxhesk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2smjvuwpb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nmkspcii.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yvptjhbu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gnmqwdpk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iqxtjpwp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2berzhmst.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lmunvgti.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2phudqyhb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cjlhyxuu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbozkni.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qbfgygtj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jnyetyab.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2aqeeacez.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ownxhejf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dlztukeo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qtptdelx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fiqisjwj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mgutfnye.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jrchxkmi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvevezyo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tgtlhlyz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yqlhhlcw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2misteraz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nljjpreb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahunzfzb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wvfxhgjj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xizltrln.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dewwxnvx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zecgswld.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2baffefdl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2elvsyesx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nephjxrq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lnxumsir.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zzcblzme.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lwbjuejh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2okchkfuj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2euiacmid.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mzlbypbh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cudhjpnh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2liyldtsv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2puzfugry.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jzbvdjev.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ynrwcnux.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqmksij.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gochbxck.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sdpbiqno.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2loxzryat.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jhdcfvci.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zrjjxjht.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vnmxjcyi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2poylvrzs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hgjfduox.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wmbvgyif.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2mppvygaw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2fhdarrzo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kfbrguqk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xfdbykib.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ucvgijhp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bceovocl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xkntigmx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gohvymge.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hjiijkew.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qajjglmy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ishwqzon.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fyeiggdr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jpqudpjo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2efirolax.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rgbtpcgz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cvqghnhe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mgtevmif.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sfwdmjhn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ehgpdiga.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kjzdsdnh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kmwslabi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wxfayeal.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uomwlbft.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gztohpae.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwrzxnd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gvsojdqu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wgrujjzq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ymjhnyil.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2atgzxqdd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zdzqkkzs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iovvirsa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2srjtanfq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zdrlcznh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rjspwwou.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2womfnogu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fzdpyqwt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2itmppjov.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fjchyowh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yecmzgmu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vfpguynk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gqfnmmja.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cemgcdse.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fjvcflrm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ocstiifc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bkcmlzrm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rbikpuji.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zjeiqrbu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mkxxtzal.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xekcwprn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jzodrhmt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lalriaiy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2iokjvivp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2neleqowl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2obcnlbhk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qvdktthv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vzmphvxh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ccohmzfl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2igvhoccj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kfargdgn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2geqsokga.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hjpngsxq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ayvwhyfm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlqkmwm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iupwwqne.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dkionbkr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mnjueibh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eljsonzw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dcrggmnr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ttxevofm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vmkasqef.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ukjahnhr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sjdhgijl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pgqlcdlu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vcbszcle.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2quxasdqx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fhxcqpov.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wxvonzql.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2klfojupi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qtkfjbpq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2uyvdtrui.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nxgitiuy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2aajtalbk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nztktkyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kkuxnvqt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dxhxponz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcztpcde.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sxaeohed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubpqhsih.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ocydiumd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lvankktw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ruqtcaxz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2behwgcws.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lvedogjp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmkyqs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hrzznhgc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hwrrxxxj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2htstyway.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mtqxhesw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pfqdaxtl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pyibgekn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2nubzgosn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oooxcdnz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dfezeivh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hkjonrut.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qwpnpnro.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qkqbvtqd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ushgiuty.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uraciclw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2grvegive.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zadnsqsz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pxicpqwq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zzwayxvm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tvzoomtg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2dtdabnon.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mllkueph.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kqxprljt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ijykiayg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2htjwpjnt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nebjoeuk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nwmmtppo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yiucenhn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jarzpmya.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xpfwsnpq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2itgxphhn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xliijlix.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2znzxweot.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qotigojg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ulibjiet.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rwcppnpl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hjvrybxa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2knphjlkv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hgpcsuie.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tsennbrn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2tjkbpvhn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jdnyevqp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2pxdeggis.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2puamleoa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jgxsfzwy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ummdwumh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jwikdtqf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2plcnudny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qciwrcjb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2trsyemry.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2orahnijg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iottykaq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pdohpzzt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dbahfclo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nctywaax.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2obnpbymi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2czzeibpj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nteaevik.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2znuewfft.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bdfremag.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2creydosc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gefckpxj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jvjfsjvh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gjbfrkdq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kttgffmb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vzxqahsy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2fliynwpk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2oqqbujvq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ydaczhju.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rdosqlho.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mpwsmthb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qqecqehd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pxftnlhc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tqchvavz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2muypzvfv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2znproqwe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxpicqmc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ubnnolee.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sbobgaoi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2jmtwnxop.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fwdcsdaq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gidmyozj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xzlqxohh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hvxndaam.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tnljvwrc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxhadkkt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2twdapubk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxxkxbqv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wjrymhpb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grpxbkxj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ighngydl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrnzctza.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bvllwdyi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ooaoarog.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bnfdrtcv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mshtygme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqzboxfg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ehaowbrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzwhbhri.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xotafhyp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xqiptrnj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2aduxprrk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lxbrhtpf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2lukqqizb.html


<!-- 参考信息 -->