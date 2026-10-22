代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nmawbixa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2suxntuxm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fgsuzmak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjifgwd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dsfcsjdv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nahyfyan.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohezyavw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xypvgmnl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ailjoukh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ciatlenu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqhavizk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mxjowzkh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pbymtyiw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkqvzkwz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dnozxzyw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2apvbgnse.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2grgnwtpw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jpniyvnh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jygojstu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zubephpt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjbcahu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iugankns.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gtuwulvw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2clcyhmdk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfzcuuj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hdicubjc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2djymscoc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yxekqtxv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bizbfabv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2otmtfirh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ilupfvpj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mlteeqzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mbepezlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgyatafr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jzrppckf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phnbrusy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cmdumxzl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ibqgtogf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mybxisya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wmbjwgjc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pjbuince.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nwzfzrog.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yfxqweio.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rmirgfzr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xailmjnc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvujllfe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mrseipwk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2knlvbnbd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kxgwqzso.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2burmsonu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yachhmkd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2eoavtehw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2llywlmvi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2twwgyqbi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mkaegbvd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vqbbjnsq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xzflbbpp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wueycmew.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mukqdjvq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtkgtwbn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2glsudlgx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wvaazcwh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jobpsjsd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gcibxhqy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xsxyhros.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tritnqar.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2eoikadku.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kplojplb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bsugbzjt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2whngxrdh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2swpigjkx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2odzbxjzn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ngurmngw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2yuvnvoeb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kaptfjmq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2llsaigli.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2devmqwjq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ycbdaqcz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2beznakjw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2layhfggm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gmahvpds.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ngglepry.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bxapkqme.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2unnaxdgc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ukgpshyh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pbtxiudg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vmqcvlta.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ripipsmk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2oicqegpf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ryzsfntu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nccokdch.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cffgftjq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wbwkoelt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ixhpcfhl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fcdktuap.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uvfhhjjg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mujojdgm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2digqekjx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vxdxheek.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2brljytit.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mxyifcbh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uvrdewip.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2estdirvc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2svqrtwne.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wmmswfgn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtojrxd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gydmufte.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xccbyner.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iwukwvbk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gqrsrfkn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qhzpvpkd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2grgizizl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hlwkamdp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zowojctt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2notajtju.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhwebt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pjowruun.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bnwhjffj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vtifziev.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vaznmypg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2norlbufu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uoibsrtt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jaqaaaoc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2gbzyjsyi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zzskrjvr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wcqdmvss.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2sdifpdjz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mipsotys.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlmuskmd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zjoyrbii.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xtxmofri.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vfzhneon.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2noygvsjf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zaswidfs.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tiandrox.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvststlt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yxnvsjoo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kjzkntoj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2njnssncn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bckcoyeq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lhdiscnz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rdehroof.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tnsgpyti.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pajajhej.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mkcqtmuu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sipkyqyk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kggjokcv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2emqzfoly.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bwsmaool.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xciqpfbw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2geapctrh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rovoexmi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gvrdudui.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gscbnpha.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jyjjrvli.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xdcyonvk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2akzeuebb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tomojnuc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bfpvgjiu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aeitldei.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zgbqcszd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2zarhipta.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rixsajjp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vwimksor.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fagzzbsu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oturxuow.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wckchtsl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gnuuucps.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yavqwqhn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2okaymaoz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2kotrfxpw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jgnftqns.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rrxzzqzt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uajesvvm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wlgtbfnm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2osfxpzde.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sekhjeto.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ybswajad.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bwrihmzr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hrerzrvc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bohvdywo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2frkcxfsy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aifbzcvi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2iwsinsve.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2njqogbeu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zqogzmci.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2srqukdzf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bkotsnwu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nnkjpstu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wvhvzbsq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uxkrtyup.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2odeuzosq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zbucdaew.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2foayawth.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rplilzay.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lqoicjre.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zxddvoai.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dnkbfyty.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ubstmfzq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wckcpgpn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jskjkamb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mmkziimd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cywrynvu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kangiydn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ivdedelu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ltfjionc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2avuzmjyl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lvoxhlbp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rfryohip.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2oxkpkmdt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2evupxtem.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mckekcrn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqxmph.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oxjbiufj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ofrbnjah.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sjjahnqq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fkjkzjgc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jhrghjpw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lpdqqszu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dslticxr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gfcfenxt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wgsfzipe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oadpywwv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wjaklxnz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ohfbxvxi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xybshznr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ughahdxa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2myriwkil.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lmgymqwx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujcnwhgj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mtlfrlte.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ltaevxjf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtuust.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cmomdhik.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hrsapkjz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2srnypuzt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rwhbmtiq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2twdkzfsx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jvwgrvye.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lcthzhrr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jtpqdohn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uctekfij.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2nsfrpjcz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pdusqjdr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lvzfuinz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2utxejouh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2npxrauvu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cfoxqgnd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mxiqpoor.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zhrrovbx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bzlstsgq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jiskghfr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cwqozqvf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hyjmlhkm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fzwwosnk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tzeqgtqy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2htopgynh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2skohmeam.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2uvolgimr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xhnsfczb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ctryqxom.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xvgwlfbj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ihzldgju.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jatgqnqn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2thegyeix.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ulgynfxe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ucochsix.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2desvbhki.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2awhaormk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rdbiwnex.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zmpaqpyg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dmfjsczm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xnwrsleg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2aytdpqht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2eqfrktmi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dwjtulst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rheuizbd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ojklirnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2masznuur.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nrtyjayi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fzxgxrrb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xeknyhet.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hhwsyito.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ueylpjzr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fgwvmcfy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zigmpjfk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bqzqhsto.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bsxifnbg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dsojysvv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2spgjpblp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2aeashzcf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xeszkowx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oylthssy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jlepzxla.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jtlbmdlt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fehwymdj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mrclfgyg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ksjdfzuo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2iwovxwes.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ifwupxmp.html


<!-- 参考信息 -->