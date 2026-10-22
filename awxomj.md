代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mvmopzes.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tvvyyuwp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyhdgizu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jbjgnudv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jcvesjio.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkmygkde.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iwdmezvi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2eqfyaseu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kferdkcs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hlwulafx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aadltztf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mqgirhjz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vputvmup.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sxtobgtv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jsrbcusq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlepyn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2azrgbvey.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kbwuvqfk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2njdmcclu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kmovbmbw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fvxmwtoz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydmunmym.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbglvqym.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hmyddevr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrapgrv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pwqwjnzg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sxawnbfk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hpyywgtf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gzrmkvwa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ocixriqc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2owpbiwwr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2adsyikoh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uoevevap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxpexkcx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ymnrkeck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esfmyzml.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pphkljym.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qkgnxiwd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pxsutsnr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evrvjvfu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2glvlxmrf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nlutxtiu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qsseigew.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hihehwin.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vbuehzrn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yiacyywz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pefqhctl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cxilhgzi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tukzocbm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qkbnowal.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pggthnsl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zczajxul.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2slvwiioj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2riowucbe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wlfbklzh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ffcfnhrl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ybtolfhw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhhxawd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wbjkpqjp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2uboapwge.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsjhldlp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkdkkwq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lyepozxf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2avkyicau.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hghwcwnu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2idtsgqys.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2aczrdjjy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fqewdbyg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2aeuuizbo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rxddjxvn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2flsmnshu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wxfnazkm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2adqxjogp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tymekbqo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2psttjkik.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2yzyehcrh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fsmimepy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2btmhzadj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sohnatmp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hzxvwylw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wsdtjuzu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2oysgqeug.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kckgstgm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xsssckgu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mupocupv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwsfhit.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jikmedwv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmhqpmr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fdanoygp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qnuqgzxi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2phnavobu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aamylvlq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qfyivodj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ibfbnpwq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nokwfrob.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xevehaul.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pqttvdoo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ckhrbpkx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aallxgyy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dblccvpf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pwtptkyi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rniqwjjj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kaokpjim.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgbhozd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2olyexali.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqfxktn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xsksozdh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nzwcsivc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2epmyqanp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ggobcntw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2chrmkaxg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2buxlczvf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xnnsxzzd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bajuxnss.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tbkmfrkw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqvcjw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2karuibtu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ymdazqsx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dqfuylgc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pigxtpwr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wnsujncu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ipttaegt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jkszcfcc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rkqgdirv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2boagdixv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwaxzxx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tltueyrf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2okhvlbcj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tudxkeuc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ecgowgqa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2brueanax.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2imonetua.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zanrxogd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bzzygpuz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2holpzscq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cycwnsqp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ermxioir.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rkswasbf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlmdds.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2puxndvgj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lqqwpulh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mbollymr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fvortijw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lhlydtez.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kicgrxdv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rnzuxaoq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nxuiknrf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ggzlmacd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2keiqumcc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pndzhhsi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qwsvbxir.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swvfiukc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qubzwhbd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ozypsgxd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2oirgcyie.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bxfqnhpq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nmyeitcg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxpurszi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hyhzeewh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iufofhcv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2flirfeiz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2npgqsrkr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dkrrutwi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zqiibadd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kdqxyrea.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2poijylix.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2uyvbblgx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2htzojjjp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fhqoqauh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bjpmscyw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lpumnltf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bnyuszlg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lhmhqfuv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wyjcvwwd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pigepgdx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xoskoieb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hdlslghw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rxniffzm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhvrmxle.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gpujymbn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wvuvkipz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ppxnntig.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vkbdihoh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qpnassss.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dsmfrwsk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dhvbkimm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2aclvioth.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vewetqls.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mzqfexaj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2tvfcpmzm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ixwxbyjc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ehdabtjv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lbrqgtcj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2czffgkmk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vttrdwlk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jvplbwcb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hxxigwwy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zuzdlxxe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zmtyztfk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2isjagttd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fdbfekcl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ewiyyfze.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wuufdrau.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pzzrazdw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2syrzezeq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zxwvcflt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mxkevhxc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kyyusiuf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pftgkpkr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xdopkkru.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pttmztma.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzhypir.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhyrmt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tarjmhnd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2acqjhhjw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2spjlavfl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjxztgms.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wuwpzgap.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2usyrctpd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jizhiwzf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2cyhlnvtu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jpcasjwr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2obietezt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlyame.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2eywwtopw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ktycgxol.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dphavzxc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iwltbrzd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wrfxejsy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kmkecchc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ngjsctbs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bavmmyqy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2igznascu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xofdudto.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2eubgwfti.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2caitkasg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wjtwcsta.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dyoixdfz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2teqmqrxn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2anjfodrr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rmjitxyg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mpvjmakx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eksdyqvh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eorrolcr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qeeslpfz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ppnjhudi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2smddkhno.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dbtecime.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uqamhbfj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gzahiimw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mlbdwuwc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gqvltclt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fkdxfhvb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2squxbilz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nuqgbopt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2uhxsuikk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wezjjrss.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vbsbgmgq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xynqtowf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yfndsute.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hbuyrmmg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vyygtlbi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vhmxxdei.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jubkxkvb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hrpibaew.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nongposc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wbqiwhvt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wtrgyzag.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ogpqihoq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tgfwfqbv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qtyjrszl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ofkgppyd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sedjuxgs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kpzarfmo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nddsqyix.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sfkoncft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peohivkj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vvdhblsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgxzrctl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fhpntrfv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ltkzqdjt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fcdyrltf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jywszohw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2brhmyvsv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xqlkqrrw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2siuvwozy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uhkzpenc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eiqkmhhb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bgklraex.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2icdmuvob.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rutunxlm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mxvsesxn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jozbglmg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kjfmexwf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2eyceqidt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ougfxvxv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2renopall.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ynylyuci.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mtxagujc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vwvfajmt.html


<!-- 参考信息 -->