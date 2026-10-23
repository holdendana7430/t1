代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3boygyyya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqjavphu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzodontz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nroxfdvz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ctbnjxyg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jmtoqejt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lnjxucpr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gvnjemdz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hxgblntp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xfnfooch.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fekawyaq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xeabunlz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oamupvif.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3karyvfuu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3piustolv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pplbwxfk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pfdyzrzg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3arjrcosk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zctwpvzg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vgpmyagg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3brblaghm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pnagrlqw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uxdtjzxw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3riiviqul.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tmuqkzgj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggouogax.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zpnwhvnq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mwhexkbp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jwbcrogj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3riowpwnl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vimzelej.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3eqvusstd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jygqqoix.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3odnivrfu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lulgyjkr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rulebozi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vjxmcojc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzdzzoe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hjqlmias.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qelnjjno.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xqfjfbxv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3szhsqozl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kowkccsl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xmgaydxl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fuyemfqf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pwtgmlni.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3uitxylwz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kxedkobg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3slkkjilq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aprpsohq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ixwubusw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xxssjykv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3phsrlzdo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ahsrztle.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wlubtkew.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwnowfr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3skwtvzsk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kbpeofqi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zdplrezi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cntjjdao.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3doknqluu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hwkhantw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nqhkiuyj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yloptyyn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ljdkmgwv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3stmnishs.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3resdenqp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kwskdnxx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xzugcelh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tsklumbw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pwvsianj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xutqesko.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gkbposwq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fuqcygns.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pikiemrl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xaywiqaj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bptyqaeb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3puytezyq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3loyxkifa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uytavvhs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pgsoqozo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3oixldydg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3daqzvdpu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3inpycgth.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yoxtuush.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uvdiejkx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jycutjww.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rhhcsopp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3pqaazfps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pnizdmxu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ieunrvmx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lzdgyqjc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tsktmrfh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3swgvyqjx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lkitsggd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cozwqfte.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hsyadudl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gumcxutd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gbqliero.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3owqlwwzu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dzovkuiq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qetsncfg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rktcudez.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qtiovbeo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jityykaq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tsdgadhl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kyktktdf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ctqqwphq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rdbarmps.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ezznznbc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3axqfwvkr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3noslmkxp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3aetpgrti.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3osjywzof.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtjefobu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3huvxliys.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fxrzgalh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dymyfmsg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zuanqwrb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kzzpvvrn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uotoxecg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hwlmabeu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nkqkmbhi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ambgdpni.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bzcgcqbd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3okerbszq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3renlbahs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gbnwucsr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xbgvlnrf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uxrcmycl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wxlketwz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mbtjhlve.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ucaoyyvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qwjbbxaa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ikayfnrx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehzsnjmp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3uttwerkh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qcdynqoo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ptixbgsz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gebddrzi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ojklukqg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uezgokhn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jtkwdsau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pdupqqcc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nekpprws.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bnnesftq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3iegsgytj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xbmnakgv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3icecufkw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3acajbldq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xeytscvp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3swekvegs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xgbuvkpf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bvdxanhz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hvafuykm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3pholezoa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qijxljuz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3diqjruke.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hrmocakh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3neuoudxl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vxowdbqv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ajxodcsr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3anqcfkxj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3auzuzvnm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fpfeizct.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xawhlnnw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3iopilunl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nnnuejou.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dvzzkdxz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cfzvrnzq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhfxip.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iepqmmoi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mvsokgza.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3auarvmdl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kvtgzdov.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wmerctbe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ctbvsdzp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ayaeyjqs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dylayciq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mkfeoqtm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wdjhbiqc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fbbjzysf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3obquppcl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tecwihfa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rpnqnlmh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3koisqqlu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cuhpzkse.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3umavmkpo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xoucownq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xygqybcp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3psumypxb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hwhwgnpf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zznilvpm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fqccfzdg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nxmyefdz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vkshvfbg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xhilhsti.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cszjahos.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iyzpwoxo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rwdssbsv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uqkgrgpi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tjarxvnm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3enzmruoj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gtvjkapo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dtnedzvi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hkqpuqjn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3exvorbtw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dbpylpyx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jbflrcwe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vhqpxwuz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hyefiyan.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oeyokjnr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bmcbxaqq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cjhsnabq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ehukonzi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vfhqhkqw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xnemwles.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgxtgok.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fuwulydu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3oxfgtpqv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nxdohuoy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvawthr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vqnlyoxl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xdogdcpd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dhpfvgso.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gnxmmtum.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3porubsvv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rionkweh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ryvmqbtz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ekoxhuzc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sfprrjyd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3voysxegq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nyobqqxf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uslevedv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zrvrvxji.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3swtpkxjd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3txsutdch.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ejefncav.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ptedrjtq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3seaifxbs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jezjxxwg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dioqctru.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mfjaanmd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3aaqekdgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3copzpqme.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tcliougo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqtpeylc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lfyxsamu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rnmnkkbu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pgxqrgis.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tmscvget.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tbixhjww.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fkkcbqdw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ezywowgd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mzzdqhku.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bhprdhll.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ffxhzpsg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3azmehhrt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bnhwatvv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vcjdlnbi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oywqlppt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3asjdxddd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dnhtilxe.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vupaiwqj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fznumbym.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3acvvoqdl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bslounku.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uzyclyxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tidyojba.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xrutkvyv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3srecmhpk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tuywqmmw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3awomevlk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kygzistc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ucpxvaho.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qudsziyp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rduezvsd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lbswsdek.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vphtdtjr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ysndxqsn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tyzfymvg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hgdvvwmg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rqogrzqu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wybxtkzr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3baahqakm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jvbbyyth.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tmheukvz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3tmqlljrf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lwjaiyyj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3knmhffik.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dzjgpvmk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fwlyrjlb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mpjfwsik.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pehsbcth.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kloltvmy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3azyfmfsm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dxueqdip.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vcgrtflz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3znijodtt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ilklnckx.html


<!-- 参考信息 -->