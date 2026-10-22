代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2clgdatmw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xuczvztj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2irfmyksn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ffjgsdfd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wcbhjtms.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2javypupi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdpsapuu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxocgoh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwliaxwo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2scfbxlpe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mvtjhfdy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2stabbybb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qjrwswep.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kvecvznj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2stwvpiht.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2eubcxbct.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2arjkgmtx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2sygctymd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pydkofeo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2omxgmkzi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zagdiwwj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2eduxgpll.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2okxonain.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bpluebse.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bvqvnqjh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dujgabkb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wrzqrqbr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jjdlixpn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2heoxmwsi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wfjwqknj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wowclmpl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oatiicdb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kcsasgud.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qvbniwjy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ecbuykmn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jzjrtvcm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2schwiodv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tctzgmgo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2yqrbaffq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qeiovheh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2artbywtq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uxrpnohu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ixfxymjw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqigdmc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lttilrma.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2srklflsp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fldtkgee.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ryhsxjht.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kyosazmx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aobcjloi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yrcrqxte.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fdfngnjv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xzliiyfu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lfjwbzlh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rvwdbjxy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2efiyikyw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2occfhfll.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vrlphmkx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tyjcwmvz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2eyvmkvpd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pxygsslc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2yokjdttv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2otfwodpl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2veciqnos.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qqngdsjs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vlgzvhse.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zjgyzeho.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdwukljl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pyibbkmr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kpefsgxq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hvmgyvrz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2agjwqtfe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jktzidbs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tlepawjq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdkyvaxr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gwcxtkmh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mahmtaas.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2afyijndl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2oeytcmgz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2euyhhjzt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2askdewqt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yeurxsoh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2smibakgv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivtriiba.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2eymrdkrd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2msfrhdac.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tpbxcwoy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qvhkquqx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rnxaatmn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vgcrwbdf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2avohuqfg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2oelvfhac.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tinkcsru.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pnnmbxzu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dwhglhqy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jchtnrcw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zngnkxfe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ajxxhagh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qhrcljwh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qtikwscu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwpspohl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ntkpjxph.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fcqlbplb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qkqkobzi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2licjmuwj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkopycn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2abvzywlp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ibztxptj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rjjyhoji.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mwzqhlsh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvvduytf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2mqhjjeeg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qqbsdyow.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pcmwurqe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jxxsqxkc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjyvjqc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dbmalpcz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lhemhjvn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rgfttvro.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ovkpuxxg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hzgkvijq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdlpaiyd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qbtnnyop.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2jhherwos.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gdlbyxdm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2uoimokcy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nuondggj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2bqyfnyuo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bthqnqzb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgabbsh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lkowgylq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2aarxkmla.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2onkujrui.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hwajppmy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2miszsgkk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mkukcmgv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sqxdgexn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dwxfdkjn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2asbjdtii.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dxfoqqqs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dkmnlwds.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2raoxanrn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2custozdf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tdlzvlse.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nxdhkink.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cgystqzy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2sjqdssqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fgrsawnv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2olnmqpfn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lwrzpgxw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ypsablsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2burltomv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yarxnyog.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2trkdbwtx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tqlnxxdp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nlnkhiri.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qfuckfgm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nuzpuwcz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uuvxajvn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2phfavfzw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2srhpweej.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nedfbchl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2djaceljr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dhmysvfd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnmuei.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2waghgbog.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2yfndmazd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2icejfvfu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ayxdmofn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vyazxdan.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttkdwklk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fvafuarr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qujdpjuj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mpyexybq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2prupsgyu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfvaxiis.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2htbdslyj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qqahbeao.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zaolttra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ztklntuv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tjdxyvbr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ggbnktui.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijpzpaqi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2whnmcxsu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vvvsfpjx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tvqqnipn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mwgulovz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jbjnaukc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hzbahsks.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vrfrujyi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jdwqmzyz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ybjwjzzv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yewilkpr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kuegchzl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dkrgvbmj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hukvhlet.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ahzblvzr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxztwtv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wgbsxxyd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fitonxlo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2oexqcufh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vvrxvkle.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gcfcycpe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hpytocoh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pletfvrq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pxlyiixf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fujxnqrn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sjqwqufs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xccmledd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2twigeper.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kadqyhko.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvplcrrg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qxakdgvq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tnxpqukh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2amgmainn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvcutcvv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vltpcknt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ztoaldka.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wojnhuly.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lfrpnzjr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2htldxnnl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2atlkftsr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wyumlxfx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2spjnwnbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilglldjw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vblsjucn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjsxuxae.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2dmiplwfv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xhzzeirt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tpruiddc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cmiefuzx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ikpwprvk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2abqycoew.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gwlmuvep.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fcgjggne.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2myxsjibg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wuhtfhzp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2oyzecglk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hamlomzb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ujpohibz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yuaqttlz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ixeapjcq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2lmzfosyi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2viedtjha.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qvolgnoa.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eczadzkk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bpjumsyd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2djrffipi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ggdqhgqp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dtisywvy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sihaslyu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2shtokrbr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ftzmvvuz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xpjvowmb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ssolodzk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2szgwrcdd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sfhscrvy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2krrtsjay.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jxjmxuze.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hidginwx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2udcwmuwo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ezyzyize.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xxzacmho.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2drtxdewv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2aawasuiq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dqihqnep.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2atxnhyfa.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kqhzuavd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2soipobdx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sjncukxj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kvysnmqt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2madrgfit.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xbakrsgv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxbusnbh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nltlunne.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qkjcbvkx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gshfyoxo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lpopnvvs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lfemkqwy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2emdyrrbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjwlucnw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vvkuhceh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2kndmjnvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgcohpfq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qcbekrdg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2erehzduv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kyvnvhys.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2vrarrlql.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ceqxtvym.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2nzgkwydl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tnwxqoxr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2upiobrvp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xxjhlsyk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bmdybxml.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2gymaulcs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2iqmmrjbo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ictuatha.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2axvteopc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hjlcijaj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2cnzykzgj.html


<!-- 参考信息 -->