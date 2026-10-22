代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xdkbpqbp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wlnesflj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mmoknhgn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wscbgnrg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zfgjyrov.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tajkmypg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2osudukpd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kqagpylb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yigtyxhw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vtwsgtdm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cnohcmcf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qkmbscuq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mrjosclv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2aujqtctu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2avdpmqzv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwacympi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lruioxae.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxohie.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nyjyqfym.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mizoercp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mwjfpmip.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gthvjycp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xaqankau.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yfilzull.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bgudmmqp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfduvjq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fxqbczmz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2algqibsu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bhhkwpwy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2aozuuudu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qonskony.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jbrcuesr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bjciizfr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2efkktdvx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2miooeuug.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uvrpvfah.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tpmogwwi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hwiufggf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ahvwkpzq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2oqvuqajn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wusobypn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2btprngsi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qjdzbqrs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gqolalgd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zbkiykmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tajtsick.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2amxgqfxj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lafiuyoh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vufqfunx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lpjnponr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gdyfgzyl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxrkqork.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dnfpwklb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wrraaexh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yhbprvnd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rekejssb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cxdawhoy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qaslqbkq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2izprcvsy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ldowtlro.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tcvuaocp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wdjgtgmu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ryqjlvib.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bfeipflx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uedwmxqg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pcboxila.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dhntdtaz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxsezdh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fpecrcvn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pmyxfgrp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2imyxdfqa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vxlrerps.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jqvkjieq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygqkrjxh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kxfcaczs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bfzywjtk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2awsqbbja.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zromrrym.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbdemmtt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bzkzdjub.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dkgapxbv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2esaqunqq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ipxwetvb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ezmoebuv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2umloncyt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xrwyyaoj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nfidmwvl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nmrxswyy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tlyseaqw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2daiquesz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fbdscals.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2idszbqak.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xhureunu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlmugds.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qospedro.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qtuuspdu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mysfksof.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bcopehtg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nphqrekk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xubnplhr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zkprevxn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pjpmqqtf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fygmrzne.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iykrpdno.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2flqoxfjt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qsbaclhd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jktitgwu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2grjdhyxd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xohwvumi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ffzhggeb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rsxcjrae.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lxxhzeml.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fblftuhw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ktfvzfbj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vzkcxqxx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ufccxogw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2brtukwbc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rlbqrrxc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vwmfezfb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zxgorxhz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xdyzpnwv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fojiwgzj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yljsiaqe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2isqbclzp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ghbnbfcf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2doovepcz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2uorsfnat.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dthbcumu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hdeczidl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rbdtnhlf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2lzpdfkbi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cchrmbiv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uuvtjfxk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgauorho.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2czvbyzyh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2euakbfni.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wtyxqgkh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kvycpjom.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2oderbdma.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xcjqvigh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2isoxvajp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zrexjhqo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gmunwkws.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oguhqiei.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2anfkmtfn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hgyrwjcr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dvnqtjxi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2douadnhw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zwmfpmwq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fzniommk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mikpsbio.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qlzactjq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cljsydrz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lxnystzp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iyqclsdx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2japitxin.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ozlyuiif.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jozggxjh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2kwmrobyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qzgzlfng.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tmhqvejf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hrrmrizw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fhmohztq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mehzgzsv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nwbxeerf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2firyslyt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ibmwmhcs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2figirtvh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vgitcfad.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pjbwfqfz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cavgvbhy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wavufkkd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wgrqxfwg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2shfuvszc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zctxciwf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tavaqbcn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2mwtnjxhg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oarrojfu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nvwsavui.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hqbkawdr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kxvejssd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2usrxnpop.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pknmsjpf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fnardmgg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2liccrjmj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uiujgrnp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xsrgjint.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqdjbfid.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xinyrdry.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rkofpqtb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cjkcphel.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2cfduhdkx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xqgvlspm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2funqtuaz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wpbicgxi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2tuacewne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgunvujk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mzpwhikm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcvkwicy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rsqorshh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rswiaemm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2apbwjwio.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dcygfddi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2obnhgvko.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xhotgyqo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kkvhhede.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dokyhsyn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2syebjwfz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qmykcfpy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2owhxcreb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2owfgaoaf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2vjbnkect.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sqamwuzr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xzaeypqq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2opstvpkh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lmogptph.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ayxeniqy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fjfbqsco.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2oqfdleyj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lnprwivz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gohqojls.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2byvofeok.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lkktbmfo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jqlnjjgs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2memckruj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2insbebjs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2higxjwzo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qqnurklg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rnsatlzn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wwbjjsfn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xulgozdc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hlepleez.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mhyaohwa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2meidfhjn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gyvajmiz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2whmptzwf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2uszfzkmb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zeusqchw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2biaiqxka.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lepkypiv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2zixliekb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qtyrzelg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zpmkrqrq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fwzucvzr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fydooghj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2krfmjdle.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gxlcvhrr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2miausikl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2naxflctk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2uinaydug.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2krhemgnd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dcyniwps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foiiodcp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xqjfnetg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jgprooeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oytdwpya.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kyauyidh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uflygflv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2novlubee.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2agbdxdol.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hyjqsupn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2imvftixv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nafhutfe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2bxrszsfq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2koxtshqg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zaglwnwn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ajwxyklx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gfwuzbki.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ubijexub.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uxslpope.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2neqkgmqc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2rccflobw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2myudgjba.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cnemzezk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2okruyole.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2adsbyjbd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qgsohwgq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xbfjwfgr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tjthuodk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vqfwpjdk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rqcecanl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkkwllow.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2keggutie.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nawadgam.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zenqxuoe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upswpvhr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hieokhqu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgsmafaq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sbusxmmi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2otdzvkwz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ffsevusr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2evovevww.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2flaecjen.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2itgqjrmd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlzfxcxp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ivljpeol.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nhsogwsh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fqgdrrpp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iudaiccj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2milugyad.html


<!-- 参考信息 -->