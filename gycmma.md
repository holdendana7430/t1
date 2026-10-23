代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lwlhswcw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkjjolcb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aycybvtt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nfqerpsz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gxlcgjbx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cqzbmpgn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wzbdmsfi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yjrumvti.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qykvibcw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3apujmzxn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvejqoxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zmbyniya.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tmphvlpn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cgxemtkg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jebvcwmi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zuktqfgd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3clbupxkf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vrqxgqaf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rjcuohgt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tbcrjfji.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xoldxpzc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pgqfnkih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hinkoxlj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cpldsqkn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3busjrnsw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3axbuaydd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3moxcsisn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cmygbdpo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cjfbkmul.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ochfmmjh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kduanklz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3imbbjazg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3semciaku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppbpprwc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3taklevkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peuzsoqy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ctlijffi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cukyquas.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3uhuapckd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vedaqvqa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zqtmpszk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3medarbpa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhmpty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rcvillya.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kxepenvx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ybqyafyd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3caasekwo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kdzakrxp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lbeefgly.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dtojdwjz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zdfskpss.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ukjlbmxt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ljctnulv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3exmvztss.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lqzpmnen.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rdhvsqns.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3chfbbtwo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uftiirji.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pqiibbyw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oolojvqi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vurzvzta.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xswtdejt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cqijpzzo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnejxye.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3schzozkh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3upwmhiqn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wxdszlqh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ojnuoymi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ypnalyuh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmhzelo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cixmprsw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ucfqaqii.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wvhlqilg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hsewttkd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3apftzfvw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lcgwtgiv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fvsbstam.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3avsouevc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vyczdjbx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yjhwlevz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tgbklukk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mltvseyh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3emyrvuvw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cwegtqdg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tqmuqyaz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nwfgbdyl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nhlvclor.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwkzldc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cfwgmoxa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jjbhlhbx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fcygusbq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pzsbeosl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vyzzmnko.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3isbppwcv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jooflesl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mxamqexx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3axfrbdxb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fqnaosdm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ulsfxpzs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nizjnobg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tptogjpw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3etjlgpkt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xitjunnu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gvslqeqz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ilwoxube.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzzgoyq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fvkqxfkj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3flbnweof.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nubhgfpe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cpgmdjuh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zkxhrpwm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xcgekjwg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vcfeiany.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zatbzsxz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cfxovyrr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qdyazjdj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ebqrrrkm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ruvrqfwp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3birjdcql.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzydkce.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xesgrasa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3izpayatw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jbmcycvk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xvbogtep.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eiykozat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzggoka.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3nchhrgzp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bqsvsjdo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zcbuafce.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bilwhapv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3skljwjps.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fzuqahkr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nwehnihm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qdpsegaj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dwapancs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mbfwygnk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zisimdfx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nkechmbl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ojpztarv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qsttxqdd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wmlbtlfs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qaibzzjs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3reqnjiov.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rbadpufg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dfgzcseo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3igjsnxaa.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bedkaznu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dqvgeapo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ryzzzobg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bufvjgjm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3amtohggn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qzoywkdv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhhqwndo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oljlsoaz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gtlrymyt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfuvezj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jmscqyll.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3snuqeokw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lvmysqym.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mnemgkgy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cegbeaai.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dxidqwwh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3uzzghtqn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wxzgyqhr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3beizybes.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcdnxytd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eafegmkq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cdudktwa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dxzqbtaa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bilgwanl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cgqnkcyb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bqrkpiur.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uzwqrqzo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xenecyss.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3snhvnpdo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3yjjrenub.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sbppmmxe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mykeizrz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3alojvffk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vycvaxrd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wmwspene.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3amsznjoo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3isltoxbz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ioeinocr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ecfzakpl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fxcyshep.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dgmhtwho.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mvjjnnru.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3eqwaxrwe.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bfpptrbb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fcezljtn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jxmkopbf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3cdhlmsuk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ioooscnn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ibexsrhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xasygcll.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ozrhmfjy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jlthcotw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3vpviadty.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dpzyyvvr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wyfftrut.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3khlrozst.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oweivfwf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ahpcnzqm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jspzkeio.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3icdmgiwc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pejastcf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bzjjgckz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3quwkmkwj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qzywwsxd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3recyqcqf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cgoxuawv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qerscvmg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ufouxnud.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohgtmadf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zkhiahhx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pgnottrx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vjrvupmm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3imotlsvs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbwrovs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdvcrzgd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ygstaclm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jnjvfyup.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cwkzmwyt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxwchs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lhgvqyuo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3okhbllof.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtipla.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xwowjecj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sjzakrnr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gfycfcuq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3sfipzrzl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hywgoied.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3eipqullh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tuccrqsu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xsicgshn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3igxuwjnm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pukhmxio.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xqrrhfkk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3auzuggaf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bfstyqsm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wgfsefxj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3sxeebwfs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kboskzrh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3sogaxflk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pjyrhnlw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rebdjxca.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3moppixxp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jaekymbf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ppanxtam.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yamjwdyp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xknifjvq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eaugmnfv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mvnwpzdy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3usemsgxm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cyakkftc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fswtsauz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jbkxjsax.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3almtbfvw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jvphievn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ovnmygja.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwhlyij.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvsbkjzd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rtldquyk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3resokpvu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qdsfdisa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qztfcxxk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwyuxfeg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mjwdanfq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hrqaxyff.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3edkdtcva.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pfjchfom.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vicmucpf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tcuhdzkb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lmykwnax.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pcuwcwbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxipvovi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3obfrlrgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptrujspu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gminkmff.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hktrptnn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ulymnexy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3saqmcecu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3biehqsrt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ekvbznpi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ncapvrty.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vyahjant.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bwcroywz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hdclukrx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bjsszzmp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mbqvqdln.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fwjnnpdu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oimdbemd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxmapq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3akhwskdp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zebwpdyh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3czjsqwie.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yhyzngpx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hfdqiuju.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bsnrsrpe.html


<!-- 参考信息 -->