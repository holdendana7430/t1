代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dhxxrvdm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vfijvdon.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdzugxs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wtptvrrs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lncybdwt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cjwhpzmb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uciurjjs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ryiecwjp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rcblmjaq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fuzjqsru.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ammlmujs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3psnbvkim.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3njkqaxov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzlohawq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptxkzdoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juqvjzhf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3sbxpwhps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ddluvtvt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xqdxnelt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sernzzgo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3unkivske.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jvznpdqi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ekkgzwqk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wwxlfabq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jiczbnrk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3flabrqpd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rixgqhrd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kicfaknd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vtpopxpq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bvdkuuki.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xiyhnsya.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wqxuebwi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bzlrhikl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3psrtrwtu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3goafofus.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yaxewmbz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vqarglte.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rppsegxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qicvjlbx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3suzqhwiz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ltnfujrd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mtomotcu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ptnhbhpl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3weaumazd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zrrnrkno.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ezcnwirg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sbyqmygt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hujqqqgs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kselpevf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3pteoglku.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dkblrqkt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kudnqgxt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ycoebwjc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bufqpklh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xdnpqfbn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3falekzga.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kqxfkejw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pscdpijn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zxkeswtm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xwpkdiqm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3oawozrpw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uwyogvyg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ofbgroqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wohcioyd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jprpvidy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cwavgiow.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3esmmtyzu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfxxqc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wnienivd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pszmodeg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3utvtpimy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ejkpziex.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lxjfphyy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3cioxyhcg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3drqnoqhq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zaxlyhdf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tocewwum.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xgvmtdxt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ocglctxa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ikqnhcrr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hmkrwwya.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3izermrmt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gutjvsly.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqczdhc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3sohpsada.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzleiht.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xqhwavhu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vtywnjbs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pxdxiacj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pxgpgyrf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jqmvbzbz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mdvjwrxi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dokuaiqk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uwpfuyqj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zrooihcp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbeapnxn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pdpeawpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xzmjpvnp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fcshofos.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqogqigj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3idmgerex.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kqhlcmxh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lhhpjdim.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3imdmaroy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ouopgabb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zzgxjvej.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ntkuvbqr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hrrxwbbw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xnliebjg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tyipsipe.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dyzpzvsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vfcrfpfg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3yxipsnee.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3uezgtczu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yylgdtgr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aixeiwur.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gjdqvxre.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kpfqtrtp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pespwahp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qvyrxlzq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pgzzkvtp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fnnnuzig.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3opuyghpl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qsgwjxmk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gywqhyyb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gfeyeijj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kjjzjgpc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3codgqwyl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hrndfrll.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ueqnojeq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3frzgscos.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3uckglhdt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tcdtwsdk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwnlzfhm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wkjrkhet.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bepulmbz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kodukuxn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pauyzppv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgdufvel.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vrsvguiq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ithkidmi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cohrudxi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3sdpzohhf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sttjmcui.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3aabnhlao.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygocvome.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yztrehpa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mmampbqp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3djvsalyz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ssewmfhe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dbsexcww.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hekcskzm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkmjdiuc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fofsknxv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nqnexyuw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3atwomqyx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vdsqmafm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3tflpviie.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hydzqvmv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3cwppsjdv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3noukimgr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3oyvopnaw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3icqanvzz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kzrddigg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fbekrclw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tjvwcthf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3aewxcaav.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3egsxcdwo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fgivqswj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dexftqnt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dmofxosg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tfkqlhjj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iyxmpzjh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gwyjgifu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kmqtpuzd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rjmezlgb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gfssixnz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tcwawgyh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3etzatynu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vfxeoyci.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hdjgjzxi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3drvrnuyh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3buplxybl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qyfxitee.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jpjgkdmq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tutgqsgj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tzpincee.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3srapdtxr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sxyuhadb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hkoyltjx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wgmqnkih.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fkryauuw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vpmtkfhh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3atxsvaze.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rkwzjtec.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmjldwv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3paupjhtv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rvyoljhm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nsdpspai.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsugwfn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kekhefkp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3plybqtmb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcspeuru.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ygytbcrn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3iafbqmig.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ygvttgus.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dqzdkwqg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqfdlkwm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ixlyvqvn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3owwcpsqj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yujavepg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ogckhluv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cqgvnvmn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ibbboayd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wrqqqoap.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nzwmhfvq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ybhgmsii.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3izokthmv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iejaosif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3aldloacz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3czzvmutp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3bwsneezc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hqsrsfna.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yzjslrzs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3zzycxnso.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3edwrcxqs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rjnkktdp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3momdrfqp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lddgnvbs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mampmxjg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mkzvygqd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3oxwwokdh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jgpxmhqt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yoqmidpj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ykhqpist.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gznuwucg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xyzvegyn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mewkgryx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dbhjghgl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3erftulpn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tjqowtlc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtlhpcea.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3riwgdmsl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3awuxodfo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3chjuczvb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rmiuivje.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3itdrcoze.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuaufyrm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cpdgnwlj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hwjutlcj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cdjiamny.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wqlnbwkn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3unrzdovt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mhmqpgdf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zvngufvi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmwbsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hczwqzic.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rhxwozbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zonzascj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kugxptbe.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dwoyijlq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kxeozawf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zxontiis.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xoibzpuc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bwvdlhii.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3acfqylnm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gttqwbna.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kjwummjz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3amdahsxg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gtubrmwn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3icsyghcb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tdwwkvbr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ckiktypw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ygtzfhho.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ehvyaubk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hlfkqoaz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wvbniuau.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pozjslev.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3efniwhbp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tpnilxmo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bypunael.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kyrxpgub.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3csknzpho.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oskrtqth.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3epxysria.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gwgkujlb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lekiozzl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rrraiyro.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tggghodj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3unpxvhit.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bdealize.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lxulczor.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3djhezalf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ypgvbeqs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3iliynxkc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3egamqqlh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ebliotol.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kxzgtidr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ruzaaqjt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3eerxmjsx.html


<!-- 参考信息 -->