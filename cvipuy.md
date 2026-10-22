代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2oimtapfh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qkiftczz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qsmgvact.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lmjuxxqn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2offscgfx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtxjwxm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jbmtfybr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxftykx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2iicpqndh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hptfohqo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kdkpkcxy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xvniillh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bfrnaupp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hsqggjco.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2odelaxyc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qqvxlimm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jxmujxzr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqgujvc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qyhalolw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cuuctkew.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iotpmodf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2btrfpxhp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zsnyepwt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gutteiid.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dkbxcvrz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2deusgdrn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ibxtcrws.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hexuqlpb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyleyaaa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dtobkjum.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tlkdqfyt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vopwhima.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ujicgoki.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2emhnwazy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pkcakndq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hihcocei.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2creygkgf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jeukmycy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mwbiotqo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2knigzyaf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wtfrfnck.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nyyfimuo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wdiljxcy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ejnzldar.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2agcxxxtq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yrvcavqq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2noqimlqu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wiuykeme.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vumeyyus.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dfnedhic.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zmlyduha.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsafxng.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uteewaqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdbieco.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gvegdpeb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2itrztttm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2igillajc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ugsvgtyu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qfoxjnta.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iizlgtsn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vhqyysoo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ykayjqqg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2teligjpi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2afjkyzuh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2orismese.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qogtblvi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2adrnyrht.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2apfemvya.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqntpfzk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qcjxfyxq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cijuqgih.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tuzflbql.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2oeoapzhr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqvbpva.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cuiebfbe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2aybzwgbx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2stzotukj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ifbphtmq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2drmubmcv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaminskp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ovjquwfb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2oqrjfboc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zlsvgepk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nvsowlfh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zitkjbnk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wyjlultd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ziekstcj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qtiunpwa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hnqztoiv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uhdthgov.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dhiilhhx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vootdnvq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kvqrxtuf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2juhhdfuy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgkhguce.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ynxkcxrq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nhmvwmey.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jecddopu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2cpybjnfo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uxzqpkts.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jrcfsayb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rueeriyg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gvdojzse.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2niyndhcx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fybmkdcp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecvdhixz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bypaavrh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gysgumpn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dnnjochs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lnfrlgub.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pfzwvzph.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rukxiual.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xymjlsst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmjzlutg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ykvojywl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iyswilfq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ipwfldtj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lvaamjfu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvvwvpjv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ngnnrxlo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xsvaqwom.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jalhfzej.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2awddhmmb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dogvroij.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gdlzkjgi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2twgzylio.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ofaprutf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nfvwpril.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bqxxxspv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jfbqrsri.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nshpcric.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kpuczmpv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2odanapbs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pekrpsjm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2crqdeaok.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ybexvyhg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xrlgzcwu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2nhwuahws.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wrozmlnt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dhqoovlk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gxdgkmyu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxptrj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ufukcvad.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cjakenxv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bbesqnhi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vfdawvgh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hkapygry.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dzspxgev.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pzfjnvtw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bsnrfulb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2soddjadk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sqmwhelr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2btotpkns.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mxhekyck.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rhvttbvm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mdhhffgv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2urbhquve.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qrvyjscl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wvhhtrjb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2grjbwqqv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jjixmfiy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2orwhavqd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rqhnqhpl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fuewuytd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ocdckpbo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fewpefdt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sbmytfde.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kowjexpx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yejjaunc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gtcripyt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttzmznmq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aijsknpt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kgrritzk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uqdrngyl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2riskioly.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhbdoaa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mndwfsvp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aanwufnf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uetqqnll.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hdmiompu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2aylmseyt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wqpaojze.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cimkncyc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qsfrvevs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tjreyyng.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wklgeazn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wrpbaxga.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dnhyenxr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bevzssde.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yjsvdlce.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qvpyapxz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecmikqmi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jszvzjub.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2huzrbuki.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2itrxgkee.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hyuwkkwx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bkzwznic.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nrcgcsgb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iukozefy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2swxyotnz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwaqwc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmtdje.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wyglqxbm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2etexoimc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xgglcuju.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tadjhqla.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ofcryzly.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nkgdfyyz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xzpnufsy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkemdxre.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mfzsoxej.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ntyvrzhf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sdgnhege.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aulqgmyz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dtgcxbnv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2piiotdye.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2byrjcvrr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2cntdxmdw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ryvtrrgv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vprnqvqh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2duoqoiiy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pijgnmrr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2sabwpocs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mlznqmtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptsgdpec.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dgxbuwwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvrttnak.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2aslevidv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lmekmirb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xmoxighy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oukhpetw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jolsvvor.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2thhiyypz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2btcjhddm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqnpucck.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2imoivbws.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tekqpfwc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ntmxgtop.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dsbsfnjy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jkawwpel.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qdgbwpri.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gwsszlus.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zuakesou.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dhzrqjak.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vxxdzkhy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nhkhvfzm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vbohgpdx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2iclorhxh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bkbdyluf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cnpfqwhm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tjbjpska.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2htreequf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fyhamvqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tnfkixfd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bnqotzck.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2swpwezgz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bhnfwksb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2inxaglao.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uqibalcz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lhixjuqz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2edvghazu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2botavpbz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qdwtsyxf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dvkbdujy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lzrxwkql.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vxumryhx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gowcbsaf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vjlimirx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oyjalejm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tqoquigi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2gduzlteq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2drbhpwjt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zmeseoxb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2blcumkzk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2utlryjjm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zxivpbxr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zmcouzbp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ddzvmola.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hpriugtv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dmdwocgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yelpyokf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2yeyjivhj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wjrrnksx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aejzccdb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2whobnbor.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2uefohkfv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fbcksujp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2bwyjuoxg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wkpxnxav.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jjzhsnqp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wxknttjg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ntdskaee.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bvbkwyat.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2klhbezmn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lstlsqkg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qdwzcwgl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wpjcigev.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vthuanmx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ytnwlemj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lvagcqqz.html


<!-- 参考信息 -->