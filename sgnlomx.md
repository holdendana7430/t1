代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gdalxjzlr.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbxxikazy.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gehnmlwnv.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gjkmiiegt.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gitefyuje.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsevvdrkl.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gwwicxwof.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glcrkvcir.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gofmtjixa.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gegernqci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/glnhvwlfc.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gbdofgsus.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzabpjzat.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gjsfvumru.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gxntybczv.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gihcofiuy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/glfucqrkl.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gzatsrztj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gdomojbdl.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gchdeilga.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gjmhtsfjb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghtbxpify.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gsdjxzvji.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbsqsklmk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggchjqzbo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gtjgdynay.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/grxtreheo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/ghomhrzgc.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gxcrqfrwm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gclgayxdt.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gucplohyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gabmetjys.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gtdtyuwqk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gxtuaekpi.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gsucuybep.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ggxwgzhox.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gnaxoukpp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/glthubucb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gusqfreuz.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gofzvwkgv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gmkjtcmpp.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/ghgukenky.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gdhixhkcg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gwhdwfqrf.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gkxhowciy.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gaclqlqct.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gpottrhtv.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gmxvvmxxz.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/glmudmwkf.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/govgpcbbl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gntowqsxq.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gepnlughi.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gtedvgfym.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gotuamyvk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gzavlmlky.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gxpitqabg.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gkjuilfbg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gzhxyzvuq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/glnxmwlxy.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/govfmwktr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gyvhydrya.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gydopkusl.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gidwumdoo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/genodntkz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gzjzlicqy.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gksxhbrkd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/glxmgeruh.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gayhzkbgd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gmtacvskj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gcotjgbpp.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gubudcovr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gxfnaxvdl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/guztxdwic.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gzffhdosh.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdkiqrjkg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/goileofxb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gdevcnudl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gkzppdryz.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/guvsdclvh.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gvqtvoesb.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gywayxjrs.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gawpxtjqb.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gilldjmrh.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gfsenqsxc.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gmqdlotnk.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gincdcuup.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gtdbuotfi.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gswyymvnu.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gzaiewusr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gbhqgcihv.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/ghtvzpbel.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gxjlgkvvu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gqocfjaki.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gisujslvg.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gpvmpjylc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gvjihogkm.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gewevqlfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gpsrzfsar.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gjpnfeqrn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gdptwtsxe.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gfnsedsdk.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gqhyfhutb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gceyklsmr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/ghaeqefva.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gzjgcethy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gshzgglst.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gfniggymp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gutdicbct.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gyopccpsv.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gwkhewdxp.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gptaculwb.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gljvurtcf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/ghgdsbsrn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gupfewbze.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gqvuxyyxg.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gcifmzknc.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gzqxvctnm.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/ghwmxlbkw.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/grnihbxvr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gwkqobxip.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gtuxdfktp.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkmhwri.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/ggkngpxqh.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gpmfqydrq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/guwpwabye.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/ghqfmlwky.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gmgewdtwr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gfknaasmo.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gepizsnea.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzpaqbuhl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gfwgprxbn.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gjjgzilsm.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/grihulsac.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gevqhjzit.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gbdhojtar.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ghklbdoiz.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gfhkdugdi.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/graoeyhgu.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gprcuorhx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gobocqavg.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/ghjbxujrk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gtygrxizd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gqhtqruzi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gbbrhiwin.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/ghzcfcsbc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gqkorifwd.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gzwqvqyfw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/geclmwrvh.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gjmlhuyjl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gozrddcim.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gljwvjwrc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gmccbrdpx.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gxhtnzrhw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyjevjhel.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/geaepafrh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gjcgibwdj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gfkwrjazr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gbwxreuva.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gsprjwatg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gflaeijra.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/geibzutji.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gqfwkvabq.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gbfbworzi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gqgvxhalt.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gnkhqthvx.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gwimwgkwd.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gqnwzdmtn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gazdzeidx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gpwtsnlkj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/greblzdju.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gpfcbljkw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gyqclbuqg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gppaapszr.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gptakxwla.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/ghpskzwot.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/giopxbtrh.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gdvbfwvbv.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gmjnoeksc.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gkagteubg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gxkqblfxs.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/ggpdqatup.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/ggpiprenm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gjrothbrf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gxsjiorsp.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gozwpubrc.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gtgrambxc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/guorqesyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gnfuavrvc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gjvcdxbxj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/geaktaaqj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gmleqnapr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/goyiiauvp.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gzuqhyjnq.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gwbjwnbhg.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gdzvxfuue.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gnjkhxxrc.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/grozqzzwz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gsqmbxdic.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gzyelwsxc.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/golnjaqmx.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gjsuavrwh.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gghraakhn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gykagsvxe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjkczvmlm.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gdpcmuysi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gaudqiymr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gpacgdlho.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gwnfapppo.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/giiipmyym.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gpqlafcvl.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gsigprnrl.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gveqxpcvu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gpyqsreeu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gvursiqod.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/guvjoszkx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/godvufmpk.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gqpgpneyr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grvvedxni.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gjqfkzwmw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gpcjfpdnu.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gpvmjxsnd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/guakqqblu.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gqhnpbkvj.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gzineghtf.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gkoywnjqt.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gcbnjolzd.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gwvzfkckx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gsfzrfomq.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gnvpbwbim.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/guscivqyk.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gmkomvwlr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gzppmqojq.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gxmhxtmdc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/ggmzsibym.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjucxaksz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/ginevtsyk.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gfixmjewe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gdlxatlzp.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gmfsvazym.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/grrdocpjj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gzptzrlpl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gmpavnuze.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gtkzbrqjd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gxyimmexu.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gvkvwvdes.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gtuzmzmtt.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjrnisc.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtyacjwqg.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gduqtnhxw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkwplxxtp.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gjhfcjgdh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gxhaeimmz.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gwqkwhdfu.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gomzrntkt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gitaqmcbb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/ghdxiezjg.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grswktxci.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/glgxpffqf.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/ghztdsxzj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gctigklqm.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gavtwxryw.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gykoequup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gcnfhdodk.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gwoncxtxw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwppzzxtk.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gxhophkqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdyohrwsk.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gvdifjhiy.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gmmfggfbp.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gdpqtuvnl.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gigfddywt.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/giznrkswp.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gzugjahoo.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gqnxkkrft.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gimznwiyy.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gmfbrowcc.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gakttwrgm.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gpbxbcooe.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gssdjaqvg.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gehflsgxt.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpqooxnqu.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gwyzybdzo.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gzvmqawwl.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gqwzureyb.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/grmyveyiw.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gawyabmvx.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gatahzvzl.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/geksybavi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpfjdqttp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gshzaykce.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/giixxvezw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gpeokfosk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gsqcynacf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gbwoaeazz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gzngrftcz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gcdbsjhbm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdmulvexr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gempunwmw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdkzsjick.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gvewgyxxp.sHtML


<!-- 参考信息 -->