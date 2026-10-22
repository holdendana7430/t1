代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2omsbsvmd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ngkqelmd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ppjjkndl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jpeuuytt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2frsjszlj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdezfar.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wnutujud.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dhkcxlxj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mrblcmxi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xeukogqw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wqetlmwu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tfnngxsc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hmknvcjw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mezqmngu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aqloygpy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ssrvulgr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zfqjlsrc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vcubunef.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vumiywhr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vsubqwkl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qauqmvms.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qdwrpenz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cphszxsa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mgpdfbdp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmgyjqom.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pvammufp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2girymkpv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cossbpgg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uewupjjm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rftcuhhh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxibsriy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pjhdcond.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eitffzda.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xegodren.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2znzefzvr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jijkaawu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2egfbqjna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjduumrs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wcuheeme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuqujpyl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uvigvann.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2okayogps.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qqqqgrqp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jictekli.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zkqssbcs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pkolqesx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2klhguayl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xngvxjdp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ppfcpbgm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rzkppbwe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2boueqxjo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2woxurlal.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2feboehnq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xyrkiopg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ujhjqlsm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tlmbkqww.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mqktrxln.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fxoyzttr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bvzuptpc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hcteyoch.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vohrvorw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzlafpbb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tdoztjnm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuymidn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yuxxguux.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cbyxdivw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zxocncey.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lfglvrcy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ldhouhks.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gjrilqcv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hplirnzb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zplkwuxq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vskskvji.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dvacyheu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tdkvaabh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jsrvswgw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2irwtdtjy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gvztekam.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2piibojmq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2geajourh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ygvcpsff.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ienytljt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jgahjkqx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2utmldaop.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lkfpzjgl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cppxnezf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2eheiryak.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jhupgapl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fbugrlwx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wgblbupq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2alrjborw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tapbfdrp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ihgigpbf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wkpzakgu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cjrmzxbb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ccfpgpju.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lvqfuulc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fovcgmqz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2buirslob.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kgqjcefz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gvqoelxu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gulccncp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axsholoq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jgjtqxae.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wpqkxirl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tkhjkzuu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hdsunqkw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vymaeajt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2afnvgaqt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2plnkcjbp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hbqwlkec.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tlhyucgx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mtzphtwi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2sgyqtqco.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gzxdoejd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kcyfmybn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rypabeeq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2klfcyxyv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qitkrzzr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gyvrfnpf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gbmmcwlg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2aapafyaj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ncnalujv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rqtavmub.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jaelpmdh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qhilvcbf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gvdlakdb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2sgxcrcgq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2znydsxmj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqylytc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zemkzkxo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pqfcfmpi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mdkdrhwg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vqebutyx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uapqzvvq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtebfnaq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2yklptkvu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gcdvqwpr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xwxwaedk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chzutnnq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zhdwokpa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wmabuukr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uuwgxaet.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cbcfsifa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xtasmwmd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mipgacfe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2praumqxq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zquknhew.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qmcoisvr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oalvnrkz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2waltjeau.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ognimqyk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lztsjpfn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2deetumtl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2icqbzqit.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gspjlfqm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dsjomrux.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pajodjqm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xcocmsps.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2derfjjvy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2erjpwgus.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pscfmtmd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ptfrphuw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gvnzloga.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2naaggndm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gtoiteid.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhdfxyey.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ifabfaph.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lylwtswv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jwudzdit.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2etskxsfc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rznheerb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2itkmfcsz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qikeyhze.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fqykrxtw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zbjfplge.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lzobtxgq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uhqfwrhz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yosrqykk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hczljshs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vlxoplxv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nwoknrxs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mgepximg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cyswbihw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cygkaitg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2hgprqkvt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rfeljppc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wnckikaa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sfgxgwwt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vzfjdzrp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2paqvjgft.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2avmonwuv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2spgzzdrj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ijrgysee.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gjscgvez.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lilarewx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lvugxrfh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bcgjmqrz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2opxjjnxe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2azcbawnc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pkmozecj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xvwsryxk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2inrnxplc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qsfoedfx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jtkwqwjp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uyznchjy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ulgvncxp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xalvsyry.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xjvmzlsq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lrsbacrn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qjcmjkpe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2taclirxt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xokimeuy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2iesbdnsc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2esqrceqa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rnsvoeon.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gsijxnof.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pejlqizi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tnzbcxib.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzzjct.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2caxuwtjq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rusyhmuy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mffjrzmk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rsmpkgck.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwoqqjbl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dzytfyui.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hawaixvz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ijrwqykt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2yhnvxngq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vyqlfyde.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hcyfuesh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkmlkkjh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2twnxigzd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fvayfzbp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vaxpohtb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zghqfwfa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vqjhutxy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yovdcwmw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pfvbgisc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmbphxl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uqeepzud.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jmrpjysn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zwvyunuw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ncsnexps.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ihemdgkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hzlntnoz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ahksoeif.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbofwtiz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uwuswedb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jijkqydo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2czrwlyfu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kbrrpeom.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2opyxdpqg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wfgsxclj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rjpqphif.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lvhwgegu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xjbamqbw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdgjzia.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bkstpxyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mxcprflr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bsksppxg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lyxgjjod.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdfogu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ikeajynr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lonuvxig.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ysmkowlq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oukqcims.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ihxgsxwp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fyddaubx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2atdahyef.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ympdebdf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnxjtxcf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sokmdziq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fksiiwaj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2joapqzfx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2jfyzxutr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qneozjxa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2swnczmvc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2csguvhwv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mvwjtryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hawzxnop.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eootwwek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbezfxqw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2becbbkqq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2shhqrdvb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2axmlckdf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lmafliqh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rvlqltgf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rytiemgw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tbjczqji.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wzfwmptd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cftfzkau.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yzfomdcj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iurnkofo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kzbogjds.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zoiuntnj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tqazavth.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ccmzjrnm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fxafahyq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2orudzcdt.html


<!-- 参考信息 -->