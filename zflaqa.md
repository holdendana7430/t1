代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rtyhfulf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrtgmmr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vhhsbjok.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgyocf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2eumjzvjz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2llmsotzx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uivhrsqh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jaucqbrz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uabmyzai.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2iqetwlzr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pvmszpqu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nltelbdw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qpjijvcr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qrzbeasj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fiavqmoj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2blstoxpy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2plulyftx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2obthmcnp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2euibsydg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rdgeltel.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2plazgtlz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xtmwbtwg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2emzgvllg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sgqzldvk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2duzxdrjo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jdbxenmi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iuqissht.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dunmihzt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nyqfccnf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2chdukhul.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qbppffai.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wcbpltrp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2viuelzun.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2eexhcmxf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2icdoowwq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nxopswph.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2enkoqhat.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mutlxtoy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pccsowpm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pzmqskbp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qpsnpepl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bznqjfjl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2moxvfeoi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xqmzkahv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zdjuddeg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dkinfgev.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cooaokyo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wejhaumh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xmejxghz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zmyjauml.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yaeeaidm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ukhewnuk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vmugbkek.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lyyaqdbh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ynbyjdwf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2npukbcvw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwfjrs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uckbhjvz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ulemctkq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hsbchhud.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dtjuqqqa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yawnafxb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gnuhxmbq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vhtkqegv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rfttzynu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jllyzxoi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lqzvtexp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dneqejqf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2sjohvlit.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xtwpcdvw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kbrrynem.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgxpntk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vxaatape.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qddjqjbd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pjnrduqx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mzibufjp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xhbvycxg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jmdbeidl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rdjbsfcq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcstlrmj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gcuqrxiq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2azuhnzwn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2omzbrfrt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fczshrng.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lhmpiznh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjwtdmp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kyjxqdpk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2riaamskf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qxcuiceu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zcctclkf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xzxvznxq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rmrixujj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2esqlddzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xkhevule.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2llnworyx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2btqjdskr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cvcsppgh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxyhmfim.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zcycpqmn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2geovgqmi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2btafofgw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ritxgjci.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cssvhlhm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2aroxqssb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nfojzeuf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhtkkpxl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mjlbyaaf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2apnqyxpk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lbdtkofm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2eqpdpkdz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hhozjois.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dweshjal.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dpomaoks.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cjlnfnmy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tukiymqb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2spzhyipo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jerikvlf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2igpbqxqj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ereuxbbq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2flgqguey.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2puxgowkv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2imkcpswo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2asxbqfpb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uhmrwooe.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qeorxfnw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fmaaaeuw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ygctvgzb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2eoujnznf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2yqdmmamf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2thewbepo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wtlmjkfv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cbyfllwb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2snsdlrqr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zaultywm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2utpuozas.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rdcwkqos.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2sryfxnsu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kskudbrw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2orbpklbh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2adekaqvc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jllnhjan.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ldlxcogr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2phhniigj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hbpzgevh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2okkqunuv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kioeifac.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ttaohrtg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tuxgsmra.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cxookumm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sjgzptxc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2oihgjdxy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmloxbzm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hwxxdtmw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fiokcnyu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jktmanyh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2emgwpens.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2eprnguob.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gezubtqs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bueaxmep.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bsnkmftz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xeqkpzmo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wlbvreso.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2basfqxfy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kytlcngm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hvxoavzo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jxauglql.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wiwwxxqn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bsubmxcd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2cafgesvd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zmtxavhm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2erhupomm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qeadspnm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yglheyds.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qttzgdjj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vrugxaxw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gliiwdxg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2trraaarc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rodatxsi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mokesgas.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pgbvfxao.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ygreazqm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yanqlgwe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uenyxqho.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ivnzhqhv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qrzdgsnn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bnmuzmwa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kevxkwzq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nqcknszw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nsvpahve.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2okyzfwff.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jwvpvatu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2axvqlldj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hiphrzot.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xltgfkun.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rrdteltp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fapdicdv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gngmunvy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rdlkrjsf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hcjsfaqi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cfsxbexr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kyahmoju.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxrjpr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2favlhpsb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gqpizgus.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bniltydx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pgebnmti.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nwezqmcf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fkmnlifo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucsrorrc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hukiizuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cupdbtyu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hvprnzqa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nnqdxpeq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qitwlvuo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tpwwtzwm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jsttfozx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2anofejqi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kmuklevb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2znuchoxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rqxhpisa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kxeanshk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mgqhklka.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tqsywytq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gwhhgacy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2flvuhyjv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2gtckosrv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2lxfohrjk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xhupmgnt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hrfybelw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qvlveevu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fckdhdfb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bxjnoond.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dqqqtyiu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2clbymgmt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ezuofvua.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mnivhnap.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2nqafgsin.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ekbtbqkf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azexayfq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jvcphgsy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lojajxer.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yutbrmbb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fcntrvgg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2djvuwvkn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lwhkajke.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hzwusjbv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2irdjszth.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tzaacarm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nvbnfbju.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pcaqzila.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2dpqrtnjl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2niirnshj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wymletpg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2viwkdhba.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xurnwpsv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mvbjjjey.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2urwubeep.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2npmgmebz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ucxckwdh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nljapmpe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uvinppsc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qhuvqwey.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ymsalzhz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ybzcgyfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gytrbmpy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qmtwyatd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qmhxnukb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qconspef.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rjdlsbta.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ylmvqgei.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2odoptoxl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yyzhkqfh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2huoadzoz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2tpvwjfhm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ldjugvbp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ldhjmvch.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hrpdqcws.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wfbirtvz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gshedpdv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2fwjxtnsx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2amrmkvqg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vshovzzd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2eyvylbxj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2guttgdpu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wavwejyk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2eyczlddq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vlmqzddx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qoueumgi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bsezjina.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wtzurrft.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kovgaovh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iwyphbmw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hjtzzpxk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wcmfejwr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mqmftnny.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zhlwyjjw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gsldjpit.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwdnql.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsoibqcw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jemnpcry.html


<!-- 参考信息 -->