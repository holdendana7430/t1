代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ahbrsypk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wdpwmwex.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tvtagnbm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qpljqzfn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gzpygaly.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hxjnbkxe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aevseupt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lmpjzgba.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uleiwxcu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qrowqwad.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2sxgakkmk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xfpgurwa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2abjdcrgf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jwmqbnrw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sufjlosh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lknhrfht.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ucjytzyi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cfwmzoku.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gvomfisx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2plstvipw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gwbpblea.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bgnsywwx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zqvlyvcu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhwzcec.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zovtlqii.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2paezyypw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2czderrcl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fcuarzkp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jzjxzujx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qjcyxfhd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dknkniro.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zqeaeeah.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jwertmng.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zavqcmwi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2nupeyvrp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqbagns.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2foaifrbg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vdojlrls.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2sqvdmpdw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ukznacer.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fheyhhof.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2olmcjrdb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pklwawnq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdvqqsxd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2clecedho.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqjifgod.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sqgsyvyj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wegdktew.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqjuwvoq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jkogatan.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2shecimbf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdserjsa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nuasajzt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nfxqhlbc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jdwugjxe.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mpkimisd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cyorjicc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ajavnkzi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yyuqpmte.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kngdccnh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2reqvpacq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wnmtvchm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2oqtuzifj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2srbwcbyz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zrqudzik.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pbsnrwaa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bczrtieu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lrinsuxv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bhipyiyy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2uftesrai.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fetuaylo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akjsjnel.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jceqadgu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lxspqldh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2srkxkjnd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ndxksbmt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zmslolgk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2grilgvyn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uzsddigi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zcoxjkur.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fcaafhwm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yquzznfu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hkwpyjpw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qseihkmv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bmzhsbvu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2skgpddbl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ibaucpav.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gzlvyewk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hnrykgzo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2noaxjpfl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2spkvbvhs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rhxdjgnk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dcyxzzgt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rqpbdhkj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2monvhgqn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2usigtsys.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kvmmtwws.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hozeldrl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hhizexje.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ryuhsggc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wuuragri.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yvthfrcd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ztbvikcz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2lfixemsc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rndcuaoz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kkincryv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fuvioetx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kqikkqdz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gwtkllyh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bbnvwsbx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bsudevlo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ezdpfayb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2edbgpssb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fylfyaoq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bxtazzub.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hqkctiro.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bgwanzem.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dryqcjin.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2obvrzzit.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ixfrgafp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2thhhfgnw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sicgsxwi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qldqjejj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xbrlguxe.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ihllhvgy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wkfjxjlj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bmmzbbcr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vxfsvlii.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bonvydxg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2btqdwzmu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2crlxfpds.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2irfaprsr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hitdjduf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gqrhresj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qkdjlmek.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2foetogsf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lsfpsqdx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hndxwqly.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2utlfvwdp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2paoktyrz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2grjmxikw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qjaebvjg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kitzatza.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2scwmjhaq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2azhxhevl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eowjimpx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2deyjxrnm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeodbbkk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tszxocyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eejtyboj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rnszjkzf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rpgpsfnm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jwioandx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nvvaefwz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jptlawcb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2tkwetysw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xegoeeib.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ulokylbx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2joquguav.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qsjbfrsp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxkkln.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bqawinjs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xbzavaoa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xmjffqux.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fbtmhkym.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xggmetgp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nmbphayx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uodqdyzi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ljzlbpol.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2srtiytht.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wkxnikle.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nmicxmkp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2eisoznfc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cxixtzop.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nbuxvdul.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pixvyjwm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hrgjdudt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2etlyejeb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gdkgsxxj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kygiszcq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rxolnqkf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sbwrhlwf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfgjukkh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tzekedgn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2woskdxyf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tpjwrfbh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2yrzdgudd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2scuucjle.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ltxukaqm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2eicnqwvn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2gysqfxfk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pjghexdq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2trnvjlol.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2poignrsh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pqnpfyfi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hkkmhgzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jztuilim.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ewgpkwoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apaewywn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kliuntfj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cldmqgsr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jgqrrbwr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yvmsipdy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mjyluhsn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rgicfqgk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lnzaihxi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wkqjzbxn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xdmyleoy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2znwerokl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2abjspstb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2agomibis.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2fylrobmi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lahtwojq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nozqcpaq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ysevuyix.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2uzsleuzz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ehktbzqw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wlzlbknp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hzycexro.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2usbmgfkh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nkwlommk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ehfglive.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cqwleaqh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yqwtsmci.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2uwgblerb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ptrijjoz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rvpyzulo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uzzktaux.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrlnndnm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ekslikna.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2osdqrriz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kmjgpyeh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iuaqhfft.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gxsgozsp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zyyojskc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mcndsvvq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wdjtgymf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hjeqbkuv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jwxpnejt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2juhtdbgc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2snvtclyl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jqyadweg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ggtlshhj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yvsjffsd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2syrjbtqh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2whsdleiy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lvvfjfho.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2txghgxxg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qdxehvma.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2pmyqbfbs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2phxmgyjv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2tstrqqag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sndqdqem.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2itgzvivc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jygcgbdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkephfgq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2uitjxuec.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2bswbaemq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2chfcrycq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2riudetsj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bfxqnzpl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vigsglrc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2lbanqagr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qvhrajno.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2lrxmrznh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nfhalbio.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jqrmjglu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mzqzcnlb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2licyamae.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wcilkzxr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mfxworzp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2kscsebbs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ndxtzzxh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2whwrduee.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jvnfycuf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hrsxrrhl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2awunolbc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ityldzlr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ywcmwczq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2smzhvcsp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pcnibjqm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lhrwprls.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccodhuux.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2slmylmwy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xzoudqol.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ipvnhuej.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dzqixrna.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgnhioqc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uqadlahd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kpopgdmp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cmcmlspj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zuttikwo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wwqetxhw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2kxmqyzbq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ugwfokxs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2zhgihinj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fjvpdubz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2kxpbpccn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2appirlva.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hjsqmpbl.html


<!-- 参考信息 -->