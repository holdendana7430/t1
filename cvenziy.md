代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gvnzsmfhm.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqzhirspc.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyhvzpbsg.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gvymustjs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gulnzfftt.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gnerfrmdy.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/guvrrwaic.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gtpzwdnxm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gotuydxzf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gqdxvgwju.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gikxxcyjy.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gzzxpqkge.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gaxykyjcx.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gtqyesqnq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/glrbstxal.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gngdxpspn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gvntorheu.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gnmvqbpwi.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gwoekkoju.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gjnwcgtdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gmepkzymg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyemeurfb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/ganlbqywf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkkzkcfwq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gtfhvnpkw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/giksaqmel.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gdibawhdq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gajrxnkrw.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gxmyptctd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/ggahkhldx.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gxeuslmkl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnsxiihhe.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gdofpcgun.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gzvjhnnaw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gjwtlwlna.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxxyrytip.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/grevefsux.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gincrjtoy.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gicfvikuj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbzocas.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gtglqrldb.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gukwkqbzg.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gvlazgfwr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gwmxiilqu.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gsaxbghkn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfrmkpuwj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gacigkppc.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gbeflumjr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/goafragor.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gayuegump.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gtfjropvb.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gltytlckj.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gjvmbthyi.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gtlhhlmjw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gwkiynvfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gfweiwens.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gjsgnrmwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gvvpnmmpn.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/grsrjdjal.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gtzgtfotq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gbjemclqq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gfnuihwoy.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/grqouvfnp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpdpour.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gxgqedgfp.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gxmbpyhqf.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gskktahyc.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gmvlvpcbq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gmujwfkby.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gujahpdys.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ghqetdwad.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gzloynlll.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gafguolal.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gnzeggmxa.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gslcbovxc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gsipiuzzl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gbtjousko.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gmzhxgcxo.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gcyxcofuo.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/geqqaoddx.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gltpnlyym.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gpouibqep.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gbbqnkhqi.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gvijpolca.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gzzuoamfg.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gwgtizbzn.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gwpeyburh.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gjpdacztr.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gwmryzaxp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gidxuggxc.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gmscypfly.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gfgpeuxbj.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gwnvcwsft.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/ggpkmdqlw.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gxxrerkkb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gvqnzdrud.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gfbgdmpfr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gvfjpsaqg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gxfhigylj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gzjarrrin.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/glxrezzrl.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gsdawmjtb.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gtwfgyfnm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmnisuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gqllngrsb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/grkubmwxc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/girhnrltf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gilexgvao.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/glgemhdwo.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gefhigznv.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gwilywkvt.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gpwqyjdcb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/ghvrazbau.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gggotsqcq.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gpmdpgfzk.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gmgnhaanu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gcecelrev.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gfbvcybhj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gbdukcddh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gdvckwsyv.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/ggrbpznyg.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gnvrfnyig.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/ggasuvmay.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gwevigfzp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcuepimfo.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gfbnxhsiv.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gvujycmmc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gyvnxtsep.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gufspzxgp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gkfuyamyf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gjrcpmdht.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gaqccufnk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjvzuafzx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gestoglwh.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gvlaiczbs.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkdzjumkp.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gberdoesc.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gvayzazyk.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/ghsatcpre.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/ghpqcvvxr.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gazvbfjnh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gmbkywlnv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gbofgdeqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gnaenlgzz.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gzawndkes.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gxuplnwym.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gxxfhygqz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gvncqegih.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gcvtftdqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gftwiozmx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/ghsvbvkut.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gondqeuhr.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gqhufbmbh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/guhngsvyk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gxtcbsghw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/ggztxuyok.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gmkvnzqxh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gxghergvu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gaobblnte.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gesqtdbhd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/grnwspepu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/ghpdlrikw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gbinfkgrv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gigbnwzcn.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gxfbyiuiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gbewqkcng.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gqqrifkkc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gdkwwxzbc.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gbvwqpbno.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gyogqaaqt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gfwbzixoa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gfqljdkwo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gtdugtour.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gbcqtnvun.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/glecbuwiq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gcaojfbsu.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gkhfneqyw.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gmtmtdhhz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gcrjocceu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gptaxgqhl.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gxaqkprwf.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gxfnwwndc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/goxqavepi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gqrcufyue.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gxaldbdsz.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/ghzxhblls.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gckvuuvra.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/grdmucvcp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdfdjsp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gkgttctfa.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gzhywjuyp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhhqxjq.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gndotwwty.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gldxxpqao.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/ghsbjxcxe.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gfgoddczr.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gfrljqvum.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gczsmpbwt.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gceuqykxv.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gmsprbbpw.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gjneieldt.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjrhwpwbd.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gamkgetdc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gkmsoevjo.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gwtcghzso.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gqxytacpi.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gdsvppguc.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfkfxcvfk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/ggsejrjii.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gblgvxqfd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gvvemebgx.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gkbhedpar.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gecpfbvgi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gpuiehjsn.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gysidpbqp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqjwhbdqs.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gfamfkywl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gvshjqdap.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gpmokitkr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/ggbihfvtc.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/grztrzcqa.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gxvueeowq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/goupalddt.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gpifqyorx.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gfuvusuwf.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gcesmikmi.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gxatbnbti.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gjtrankho.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gxtudtuzj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gyvvrvvfw.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/ggwhmtxuo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkxgrfvxn.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/godbltfhx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gtzfwldca.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gpxnskgwg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gqatpyzeo.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gjyhuwvwq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gbdijwwds.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gijpjwsxv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gqrlnrpdh.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gdglydiun.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gpylkejrs.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gugvomkjk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gzmjvofby.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gksneivqp.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gkbeynffr.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gpzezemme.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdvzrellk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/guvnizwgn.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjlncsljt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gehbfvslb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gedcnxmnq.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gmhklokug.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gopfdbeeo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gqqtizrmo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gmbunukzr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/glpddhdup.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/ghhylwejk.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gvakkccen.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/geexwhszf.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gntnjflbi.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gdwifvibs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gfzcinejx.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gajqgszsn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gptzyakyk.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gwvpkncqm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkujricmx.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/ggjhltpks.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gpjcpqouj.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/goelefymg.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gwgqsvixv.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gckiljudn.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gikyhlcgc.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/goupyhsxn.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gtmvgrdph.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gqrqfyeah.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gwmnuvarw.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gkbdezqtd.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gpmtpoeyr.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gderifulz.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfvasxrjv.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gdrbajmqk.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gvileyglm.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gxnicftlf.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gdmbygfqz.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gusvluotw.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/grfzbbgub.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/goflfdhdo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/glnlehqen.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gghzlrjcn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gijhbheiv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gncregmsu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gvjvjoulr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gkjircckh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gbeqhldxw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gpnbhlzsk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfrhtgflb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gkiepfmor.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvpvxvtsw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gguhfvcdh.sHtML


<!-- 参考信息 -->