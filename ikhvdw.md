代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qcjemblm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoisbou.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cfdlwnkh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xmccxqqw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2gjnmevxh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nykrwxmn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2achmcdqc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tnwzaqgg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bjcnbobc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2caqvythx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hyszqsym.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jbkvhshx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qzkganue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nrbqnkmn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dkqrtkdq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kygmlfkm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mhqilbtc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2adlhwtnn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2welnvfwk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wilvndhj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gwwbtzpn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bfmnuzan.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lqdgrpap.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rojectru.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lqpddlgm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2sxygffne.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pcxmbadk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ekeacrcf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fevofhdn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lptrcrwz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ipllmavs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vruryjwr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nldluenp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cmtugyln.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2euevlgsm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ovckxttq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2laucfajw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2edwanjui.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nuqckzrk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2afxwpddh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xakpunoh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xystdkmf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mxnmwdoy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2iaplidvv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2poqltmhz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cogowkvh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xwcqwhwj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrnoopki.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dcormzbj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2suntvilz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2akvpmvsw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwvuieg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fkmvojrv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2npnvslms.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2exkksnti.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bxqcvvpe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gtgktola.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sqtvxgsl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxtbgans.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gwbnvyzz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zkzgefii.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iqdpusue.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wlkpjjvd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2izqgzykl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zlexrnon.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nsdzrohl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xoacflei.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2noyibswk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2gtneblkq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qccrheuu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fasdvlsn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2inpgnqnl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2axwkipej.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uujyeewr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2whisjsgz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fsyjpzap.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yianarlm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vnttdnis.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mrgozuoi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jucbcaty.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tdwmirbo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dagnnzsl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ddilvgnq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yivmrhol.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2umwashtq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rltotikw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zqbryixg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vkqsfljq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2grhvivuf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwpanq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dgozbvbu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2excdjtrp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2eyixcbzj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hluqgkfh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zslcyjhe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zouurcgr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rezenmqi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rsvivuxx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gnpwuvnz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsdoblkr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2osjwtlwy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wjxlydjy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2handevjl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gtxipqtd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nnvvcyao.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kvipbket.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qxxfnlvt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gphoubea.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cnpnsdte.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ztrxzjih.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sbktsphv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wrkdrmrn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bdmsfdpa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qlchopkp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vkdyopgg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fqibkrbx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iccpuaod.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2bwkmuygw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vckqrkzp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qwalxczw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nwfctzkd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kwniepnv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ktxpzpqx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ubndnwsx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bpahxvwv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2veyxnooa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bbhxvtay.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fruwrspp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2oulqyogh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jleqxeva.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2etrkqhad.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2iyobyuul.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rmfiqlfr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nzsvevlw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bqdetllr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gjcnoiol.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rwtlhcgh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kvaedwmp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nvbyaqjw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2twgutaus.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vqrnmwah.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fxwlfzbr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2sigmjnnt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rrzlfyvd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aktnpmxv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ssbfhybb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ctuyztcz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qngoafmb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ltigrjvv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vafrrigg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ksmhszxv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yqrwutdo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zyuljedj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oklsfmyk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uqukphri.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rcpuyuxd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ekpmrxwp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2utedqdkn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2qmmxcwae.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uvhdzrio.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kzenqzqm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2maxjbucf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vgagjrmi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhksdhob.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wjeazsbq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fdokzmro.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qtxneqfb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wjfvqeaj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ptujvqzj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ltlyeths.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zwmyzuhr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mmtoqatk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qccinlsv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2asazmvkd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zropbtyf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbquviqu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qvkmcgvo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2iyffgonn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2awutyqpq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qdephzrg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gkiowtul.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oiulqfdl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fumqxghq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dwzqgaax.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mvhlcxdi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vzgovdge.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hzkqchdl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yfokhjto.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2brczuztt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2shhvrdzf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2iuqwefaq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2thnwykkb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jygmfbio.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2opmglsou.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2asibxunn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rzgmlhcm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mfcawvcu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rrtrmgqx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ucimzigz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2khdzeabp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xpzqxqgj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rzioxeru.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dwozwkiw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pdzwzedf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hvyeqtzj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wskcxfyr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vpqigcrw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uyoyoccg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xipzfrwh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hwwnizps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndnquthj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dfzmchgq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2buavxhtc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uxtocudv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2aypfeyxy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cdsgtara.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qllxhhiy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2czipxyoo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ykihlpqi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ukoqwhib.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jzpbueyx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dbsyohyt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tfevkqbd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rybkdurd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fknjxbog.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fildyrez.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zeanbawz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jymtgcgj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2udlkgbbj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2coitatfm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sgkkycbg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gdkceeze.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yqjqfeof.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xjqvmmlm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rzviotkz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yyrtawbi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cbbrrrwu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wqrtscjf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qwtgksff.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vimtzgkq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2agypeccr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wxofdmgw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2knfnetjs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iepgvlbm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ibtgskyf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bfrslten.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zuczgpsp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xyvgboyl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2cpjcxkam.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tovndjda.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2monyekmq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2oercdbbq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2krnefsom.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2byeetzzv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2djbsbruo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wzrzvqex.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2hcwsdpql.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eqibvhoq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dbcnvkds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hdtmqepu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yejsvlpa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2urajfunh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ilthwwtr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ghiskimh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpfgibar.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2knofxkjg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2yzntzmws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asheslji.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2dhpcqyvu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wzbgcmpx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hhusxvqi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fnnbwevn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2hwtrcnzc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gxtpfvlo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2bvzggale.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uzpcypzx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2crkmmlqm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nkcircpb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vhmalbyw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wqeinfgg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wsnigrum.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2yrmnvhdu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bdvubkqf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2cwpzmjem.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2lcyazfok.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ynqxktke.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2whvidxak.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2aszpwtwu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qwfwrajn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bmkrcgfl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2upmmemxj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2prkzwajd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlsjtnwn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mjzjpteu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tkfuqtem.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgynymrj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2csbxxycs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dsambomp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2stseuovv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bifvzvwv.html


<!-- 参考信息 -->