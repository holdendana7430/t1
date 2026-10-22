代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2eoasdzdd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rjgpkcbf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wskicygg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dcysswde.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xidwclux.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpgewfax.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2swraisho.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqhfuqwf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zxewpojv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kzkmqsgj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vxsdatba.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sedieroj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qwkkhcjm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fqlueocv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vihquuki.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2chuttasp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2uebnfvoy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pubkyxiy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wghdeqpu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ivhafoab.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bbuvhwwp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gouvcsws.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nakjmqvi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmxjonb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cjyzmtcr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lkqquipv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hqetjgbu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rxymcjyz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ruabpwcm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2opdgxumj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jpvytvxh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcveerw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jkmsbwhv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fqqpzedk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jsgaqnbk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2selaueig.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ywhgdcvt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gxgtmrzx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rkhzgxkw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cabiosry.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tahovzko.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ioiiewun.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mtyacwtp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uxedvked.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ujpidizi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2iyfwqyal.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tfsldxvz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kkknwexh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cjkodprm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2egvskxfp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2cnhrbrta.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cabjagup.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zjmgzujy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2bgwjgupp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zbnvsjqo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fuchreea.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hkdjobnk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ppwttqan.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vvlxrqjk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hqmzxwmd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rttjpnam.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ffkaehjc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zlhmahra.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgxcufp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jvpjvvcd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2guemkfqi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2trpepjpi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmnhgx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ovwuedir.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gooxdeab.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dqkmoxcw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ilnoxefd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2svwzdbyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymvrcivt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckgsqcoy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nunfylvy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qcfrojjv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tlxwepoe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ozdvnvrb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2devqwtrr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2stlovddo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bcwrhutx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mjixsdlc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xubbicxp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dbhszhrp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mbjggwrr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2reghupwa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bcbsgnia.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wpiujemp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xwvcenwq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vydwtykw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vhawxfwq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bwqdrsns.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uyooefnm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2irqqkmeh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfhmydp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eksnqkxv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yiosthlb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qqitietx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sxbacmyg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mqzawmsb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zjkicyvk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2obqjtxnw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wlvqqaeu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2anvifzol.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jpyudttd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bjuencqz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rpzjuwoa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hyrfwgak.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2oaaanizp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pzrygxdq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ehlsqftv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oknmfrpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wuqkuuth.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zsrodanj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uplkxgkm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oseroqvk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yqnsqxcw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2viytispt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qjauytll.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ewgiyfpv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghizjoky.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vnzbqlrd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ecroygxc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tbbsgdnu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pcgjqsjh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dhuceizu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2osycqkaz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2unabfpyw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wqqmchab.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tuymyhdo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lsjhmcfi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hjuhsrgw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2isseatbo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qnsybgpx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2aqkmbnbm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gshdzmrt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ulxujlwx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yfwyncse.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bonizgqd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cpedmikb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2muevwubk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lsznjgjc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2czjtmalc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fkqjspqk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2afmjhetw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2aadltckz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eauqgyux.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mwacsivs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bnbmfrjj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qiuinhid.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2swwsydra.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vrmnshqq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wrssupvw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2aghumjsf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rragnzlb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hpvunbis.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yulwmqsa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ejqnumzb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtermerz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2keciyjit.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ptlfmyzt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2knglqboe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wwusvtvu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tavunshs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2asblydzt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pgobbjkd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gavbusog.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2imtwdoty.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2esehbqrq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mwbqvwvx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cqefuugv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vsrziqpc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2soamynfj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jnfclfxg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eneytzzf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2iayxgufn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zacdcpnj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dercynse.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wqrhfegh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mfetuthq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kbvprklq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2medwajxt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oqqcobmn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ditomwmj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lrghttoj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kmyayztb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2esuzbifl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yawebtri.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zdosqlxn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2agrmaimt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mwabawta.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2evwatwvk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2afkffwuo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2whggubwm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fwulctvp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qmhhisfz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jwghgpkl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hruqocig.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zrxvrlsv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rjkiojow.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tbvyyruh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vzabhfol.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nsoqelje.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2srqmjgkc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pmrzafxa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2arybbtcs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zvzpaekd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fuxrnemb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmzdzomu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2thfcftzu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ujyizrif.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ohewvypc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dujqeyep.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pvswnnjt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bciswado.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yjsnmhlj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ikhevvmc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mpcgrmsz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2shciioro.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2nqpwbfgf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gfjcxxke.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hfqmhvhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wfbocdpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqltgoqd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2peqdeozs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvisvikv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qsorlpwf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2aioiyfma.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2woefzaxi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2skegxaeb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qlhilmlu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zgglhwbe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nlkwywwc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lxqldyfh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dghrvlgy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vrjcpjrn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mxlcvvut.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vthhgfnh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yvhewhfm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vklxnhpl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bbefpigd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2myrzraem.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fmuiotzk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gzjjetvh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qlkaopyw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ttytzljo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cexodigd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kmijabnj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ldomtwgk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bixxonzn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2histjmdg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mfbtkuum.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lstbgold.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vbdoosfs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xyselhuk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oaunpbfl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wdxgvgjd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2caplwfpm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eqgpgijc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tykrjdrk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fhdrkpls.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fyhyanvt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pijcvtda.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fqfumabq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bgnpbeyy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uzyhtqla.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vipuxler.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qjkgvhzh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2afcfcjzs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sxrcqcqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rduzxhac.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jhppshco.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2veqjborb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2unxoksyi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vxyoyuvm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nttwtnkw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2okzxwdif.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qbvykspg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2mknpbgrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daazxsla.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uxvcdoqv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2obvqmgtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inykokwr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fmcylinp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2cruwnjiv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ikqwefuw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2tdymlukm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hbmuwgaz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ykpxmxgl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2smpqniyv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2hfeqhayc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rmmhpwdm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ikubomfc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2miodplsz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wbbslsfp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mtmaulou.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sakjyjlw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2chvjqbkz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ynundnhb.html


<!-- 参考信息 -->