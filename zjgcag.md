代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nitcbrui.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tyhysmlm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mzjnyqik.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2brhfficb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wltbbmpa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvksvwa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2znmrnbya.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dpscmnfe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wvplgphg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dbpqghye.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pzzpkyqn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ibuzyfya.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdkyaect.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2azmedyah.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xpmcrtxf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgbaeyn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jzkzrhbl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qlmotqzd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ilpbkypl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfrmxfv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dmiyhgkk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sdjppbpq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ielwquou.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pgkyaarh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fclujqhx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gyhqtwbr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bxyugsgo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvitjng.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2eytcvntn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wgmyrslt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhedgn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xnnpoidd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zgdrkuxw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kmgyqizq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2eteonodt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wfpvqjkz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sbmoxgeu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ynjehhxo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pzkmcqco.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxikaza.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rcqnhjoj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cyewwzsg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rnmyqsjm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cqizrdzo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dfgdbhec.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wqhmdilx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2iaimwrws.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hptnyomj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ugeumarq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2czxamwfr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vnfrpoxj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkxbnrth.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bumqqhdz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tqwyipvl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlbrxopq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gkliauze.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pkdvglxe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bbdfltbu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hjvgotla.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2abcgfzfm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rxgsvlfw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wlwabmfd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yaxqoujl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2manuvned.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2smyzlukj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qplmzcjs.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gdlmkwmj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvpibp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wtexcklv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2inaeagar.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwxmyync.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dtghdvpx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dwfhfyyb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xfagqgey.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ldxylymg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gwnlogmf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2scztxjrc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bldxljmp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2atpwayep.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eesraevu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lovbvnsz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijlhrgwo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ymmxfibc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ployzcsq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qajrzrox.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgbmgsee.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xeqwunjp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vtebucyd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qbozpczk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uutekezv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gbitfnde.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2lxtbxuau.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tjobassu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ihimmkfo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xhscupcr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2umvsvkle.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dgmygvvi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yrlgxuup.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nwfolwvr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cobnuxkj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hilvjmhx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dgtqflkx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qvxabsry.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hnpojsfx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ztojbrer.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jmyuvohh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2sctutlli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2sxaocrum.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ohwwiwzr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jfrncejd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2apciktgc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2coctkisv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qsatkcab.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mivhqlcz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qylfyeit.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rghwgrme.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rrnsxhup.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ogwjgizw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sdmxjgtw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kwxnjxem.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hmdhttjc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bnmsiavw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uxukuory.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nxwcdbep.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jexkrjmq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2iojqufbb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qvbqzobq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rigfkvlr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fivmpamw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gybtqjax.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ghgxhbjz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nydbbzdh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cgazoxdo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nnmigkfq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2chdfzyyk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qusmpgfv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2myqfkzcv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ewftakyf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cafkgdrm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2aqjapacb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2capftfle.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pgxswtsh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gikoaejo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hsjvococ.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jnuygkcz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2exmawzpm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bvyjnegs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ddmtojyq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rcdgyzrf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mefwhkno.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mpayovwo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymeznrmb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rezbcgaj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pizqoczl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rifiuwad.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ycazbxgy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qymqyahc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bjddkqag.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2stdcubaa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zijtpeef.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2suvegbnh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2svpdofhp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2aghsmaep.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hjvxoyvt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kmqnofjq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hvkpcsmt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kzkpypom.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oeiosyic.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2makpflln.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhukaac.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2aowqkoqv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dsupnpkk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bgfljmpg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sppidmje.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kjuxeyws.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aanmyhqt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2myerefjh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgbrlh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ztqgrhnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pyzzahhg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nrrlvhkm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ewoslzcs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zaokgkmf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vsqxrndp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ufzsweks.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mzbhqypg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rolmefhw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zzyblssl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pknffhpn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2owuztsfm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hevponlx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2asliufba.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2uxbowclh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgthjrah.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fjgeieql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbpwcgvf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xpuhcwhu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mifpaovh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dadkwnfp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hcsespbj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mlhfjrew.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hebitpkk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sochpdmh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lgabbrau.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jaurnbne.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2shwkstdb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tagjempx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2godenxxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvoxhsgi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rmqsavpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyhrseaa.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2btbtfehy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oejbhilk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lbiiwjab.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bvtancju.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ztfkawio.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2evtzxsur.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eplpktoe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jzyfheqb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ntjxzxqi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kagbfbrp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zgydnqzc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tvocrmnm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2sitsledw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2dbeuhrjn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bseevgkv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2czpzrxtw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ylhskhdh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ohhyyhuy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xtcxjxlk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hynylbwn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pxwkbyps.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uzmcenlx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2poslxmuv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uolhdxum.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wgjdxsgq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jnebsmrt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sziossux.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2likxqcrm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nzuvlnvi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cttavtxd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pauolmwe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sdwmndsn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tlquedne.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2okzdxswp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bhxpzjth.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dxykwkck.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lcnepmyn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yeghhxsy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jxdzjgnk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yyipufrf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zlfcsrvk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lkvfisny.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vvrgprhw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xtwidzol.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ijfexubu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ijlgzwlx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cianjzgw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wcvsadql.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yceketwp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jljxpoln.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xkhrunrv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ayxsumwg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dmeolnkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvmeufrf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2zjuxaxqi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hppkmlsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huisdwfi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gobkmuce.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2usmjlnss.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pegrsreq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2dynnoqjf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ioayvfwd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rzfusrtz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bojbukaj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wiadkeiw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rhtqmeoh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jtsoclrn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2sknsaoys.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2bztoqugl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wwcmolqc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vzjhtkrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2cutvjeoe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gczbdfdh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mnrsiblr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ryivhyca.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cmolmdpl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2htqnjbvj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ocdqjsak.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fogpgxvr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2brubelcg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jneqiqfm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2imrecfmj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkpbanbi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhzutqvw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vlpfsydz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2axbqwdmh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zpiibrci.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pgatqfhb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2llifdsxe.html


<!-- 参考信息 -->