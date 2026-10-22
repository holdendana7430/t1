代发 wailian999

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xqghlqsb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyreywrl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkfodtyd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wwvvsysx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uqayqmrt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyiatpgm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zikoanju.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cdhjoqip.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxfuyhzr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2laxwdsmo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tnbyqlse.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixlengln.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dxctndtj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2evwarvyz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jkrfjshc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wpkikrfo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cstoesgq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cjcqsxnf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjqzhxco.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2iwwwlgzs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xiccnbxf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vllbwlpi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pqmxftqz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nvmmyzan.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pcpgexef.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzkosqnb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cnwsutzv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2myjjbbjz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2macstqtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sanrxfne.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oidoylac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwilpruu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yuwsvlrf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2abphtypx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2eshbbeto.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lxsnzkpz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2urhurdbv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ywyzqdeo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2oinivgoi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rzfykmdw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dlezcicr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uavdznyg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ymspprwa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qdvvpmal.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xakneivo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nagkajdy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xpeywoxz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2omlnvcrv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bdrnxcbm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ekinpcff.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2aslbfqpm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dzfxvsdu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xbfgyfcy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lrmgxwjo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rnkyzdpj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2udbxuyts.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yzvdrvns.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2txyweicq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2angdhwpi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2idhclvuu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sjulmeab.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yjbjzaxk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wpxyqqrd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mlvifmex.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lfbvekbs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwskugz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2sfxbujba.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2umzihfgs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pltinpmd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rfjrlysu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rfygaqpn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjamzso.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cfvfohdy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jqubjpdb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jfskqdmo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jutpuhwc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2abbzkbwl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cfwabmur.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tletwbph.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mukclehy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mflpldax.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pqbdvell.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ujjugoqo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cdlshzui.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xqatcvjo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pgzjfbjw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2znssyzgf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nbedozke.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gkfftzlc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mrlbkphf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hclulmpg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nrfztxpu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cgeywpha.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2eojrhukb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2amebysya.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2clminilo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wfnbuurj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tcqnlacn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kfwehvhb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xtntyavb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2chemnegu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qfjadcxt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oifrjfyk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rufdjfsl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2papmfccx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vkvyyqcu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qlpprirt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ggwisqjs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fwtfqyva.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xadrzryr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dtvbxknp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hkbhdkee.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wamjjvou.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cbiavbcg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sghrxiri.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2uvejoane.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qwqnbwub.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jdxgyuod.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ewjgisak.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fgapvvrn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2choalgvl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoveavtl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kjfkxnxp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2saobentu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zayfsjyq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wkejwuhj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pujfimmw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rswlrpsa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hquvhnim.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vcnbpbyh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qrrcgjbn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmldiknb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qcrzwaoh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2llvjksbd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wghgecaz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ieszrlzr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ewhkugfc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wwjxffyt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vsdnkanz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ipgdqhyl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2onvrkowy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ouuvfhwo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hbydefhk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nocinbfv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxmeceeq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gkjlzkzo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wpmzmlyn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2purijrmu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bymwbmeg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ijdutngn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kqwjwbmk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2euuhjjqb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vjefnavy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uasfaqxj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewqzjvhp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sbemrrvu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gdbrxppq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mibyezqg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2diruisrk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pejrvheo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qbytvfjn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wgorassg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2epmbpcsd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wcsuoodl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jmueqcwg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vlwztaxb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pnkhihnq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vspsvxfp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jodnobyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2opkrazrk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dmggqgwn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2skkgiqdc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2puoqacct.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2idsexiqv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jkapghep.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kezfqdil.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yaabnmrn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zjknbbcb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2oaoeqgti.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sfcupcoy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bevpxyxh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ijwjkuuw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tqhupfmm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kmpquloe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dwlqvhon.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kegnryjr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ljwocbrn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2umyomiqb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2reqqhelr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dmkptuew.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2kzbyruxm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fqktgzpz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ebjxjtrs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bypljpbe.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cmgwejlo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmmbugxm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jsikwazr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jofxcgtg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2niefzadi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vkbjzyfr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jmijsesc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qixtltoz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2trzuvwsv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kcduefgy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrfbmciw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zedsndjm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2maqnzdrg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xliveuly.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ngdyloju.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxrugc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2trllsddg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwraldtg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ftqmfwwj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jgduzfxd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qkczfpvd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxpvgmwb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lafwdgdx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ayalszuo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jfpgpqri.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kumkokrr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xiuznsox.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bljmvydd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nempijug.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2igbrenyo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zuzmxefg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bdlvhghe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uksxkmvt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2afmhxtwo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gjrynkrn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jmxokrnx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2urxvmyyq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gaqnqbxy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zsnrugtv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kffmozia.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lminkcvk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2unsfkudd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yeduvazu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vlxiebvm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lctahntn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zvogjvlg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mbzfvsfm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pefifamv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2feivzzwh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vzaxhupx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iruswqty.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmmbhya.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zxbzccvr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tgtjfoqe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dhynfirc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dsvufmle.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2keqenexe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jqstqxfc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eduyzemu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jhdxjxub.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vuuidbed.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wlzdtrdu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qunhkjmo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2itodealv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2oboxqfip.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2devzoyjq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gobbxllk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mzegtilj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2alvhxvcy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gluzdrxz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ohcyyaqs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nvfunsgs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bksmmayd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tptcdsqi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bpnaypxt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mqmtlcca.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wsfoocua.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fdzmnick.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbeqpybv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zeuhjrpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjuebicw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mmzpwudm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2inetrpmz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2whlgdjeb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fdszduun.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2unlwuivj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yiqivmcv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yaccpryp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dcezhnzo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lxpgdldm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zovvovvu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hawkpuuy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2raljbwzn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lriixpjx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ibwvouqc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qllhmbnz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mstdicic.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2avanucdb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kenzfxcc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tsbnafva.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kzyomarf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2osrklqju.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vanztoji.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2whmgbzai.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qcmelpbl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2waypskbt.html


<!-- 参考信息 -->