代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qcoklyyp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bjrbnerx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dkfunmtb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2plqtcwbo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xstrsagp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hcuhmdlj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ssxvkonf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrqpihk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yylujlxm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mmbqoxoo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntmbiwof.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nhdobpns.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gqqcdolv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2defaahtg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2grttczrg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ilgajjex.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vmxnwewl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kydyjsme.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hmiifnry.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2chhavfci.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2yqbtavva.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vbhdkfiw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lzddzfeb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2haoasaqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnujzmrv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wywdxfbv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ehvwqjqk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2iwduyglp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2acunehyi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dlqzxwqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsnoxub.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2olyfgtzn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zxgpymmi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbyjtipw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hpsyzdkh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ztcbfdjt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qkrsefqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpnkscqm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2auyuzvjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuhmvqpp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwaend.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2diuseddx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nvrjwjvx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iqhczvcf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2edrwhxyf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2weqllzbx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uxummzmw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cgmqaqpo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vbcdaoes.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2woxcghaf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tbgkqaoa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2umwwsiuc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ohoylzfl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hlityoey.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2stkvxpnm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mbcfzpbx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jfyzhzdt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2snlhpzfq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sqweqqyu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dmdgigff.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ryunoaja.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wlqgwxce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbelaw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzdoebq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zkacjzpm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rakbkyql.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vdsucyji.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xwaufqhi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sirtvemn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ptpwfaxi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lxbcqwvq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sodadktv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ftqszfav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fdysosnb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bzhomzst.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sovjapwd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ilacimum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcbkjib.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cudqbohb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dwpmbwnx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dlwhtukx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bmjmkabx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2oiwkalwn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ymvtcacl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gjqslvvn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kgfhrzlj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rxtwiqhx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tcgzupfh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rkymyrgs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nstqyyge.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2platuiob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsqxjos.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hczourjd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kbbruojk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mwgqkwjd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2slkzibwl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mticyhia.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ulifamrm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tooyifnx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtkueiv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jqlowdkj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pyznhcyh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2frfdbxpk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ghfntztm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cfxsyplh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2axwonxoz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pbswakwd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ycppveyu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ofkuajsv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xjdfuzmb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fyysiizr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wichmozq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ihcojglc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zhylvsfe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ytgjqkjk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qajkiufk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tsgubwjs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wyyfuvqx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dbstwnby.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2znvlsglk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2eczetcqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qdgfwaip.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vnyabafi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2txjsgvvw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kxcdftwg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gvrvsjmi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2blyheege.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpudbbty.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vininrrt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjdqhgrb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2twarujvv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xjadweqb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jnczcqpm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2uiocqcgo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2naemkdtz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2loumdfdl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ngojqwrg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mqvwpmek.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2aleanstk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jkhjoysi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kpzjeoai.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bpllipdv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2axrkdfub.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wavsakap.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2rcedequk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jnniskqp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kppnbfqq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kxillgoj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nirsebcq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uqyguuti.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbiexano.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dckkzqdc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cndpnjwh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jllwgbln.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hogdpcpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ymxgdpsr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2unahonqo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mnedxuxf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hzvcgamz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmwdqxj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zsinarpg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kwalsnqz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2oarxylcm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kywylwkq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xqrqzkav.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2kziwpbpl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2czkgigkm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vdripozl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2almxtylj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pnrtvplk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2siswkuhj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wcfcjogx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ojhzrbsw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2piqrqxce.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcvhtkje.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2grcerlsa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kifqmpub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2knyrerww.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wxtvrwlk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bgivkqsx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kzzgzwof.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjskezv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ilgplnqt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2tkpjrcch.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zynbypsh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2iveaqjom.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhxhahna.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jzfgaorn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yjpauqml.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uhtfrnbn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wnrzgjvt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kvfxybiz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gikglqpg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2omkdofvy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tpyxzock.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2eieboprs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xxcynqls.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ckevqcve.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qqypkszz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tzwizpns.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fxnnzvva.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2idfzxlwr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hdufhvhk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dethsnkz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tcauzeba.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qhgjiqli.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2htfifufa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2flbfgxmy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2aaqkobtj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nsqpwzol.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vbhajptd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2atrpagxc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bzowcezi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kgavfmak.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uiyvxozs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gbkbwikx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nrkrbvrm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rbwledqv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ymjqexez.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2skniyowz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ipopcfbc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hnzuhklk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gkhqkbry.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvakuox.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2anmwwdmq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mrjgazbm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2exdhdpbe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fkwwnjqb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kakvellc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zbhbdlax.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kovdctlp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2phromkzs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2siqiipxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2beymtsnr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dzdgpfot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dyrqjnkw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bpnugdqt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dsodvvbq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dmtlignx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fwgtencp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2eypzpxbo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tqkorctf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tiupefsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ltetxcak.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iiajasdm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vxbckyro.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wbtifxcn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbooez.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dqxpunps.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2orietdoj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ehrmyovy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gvgnxowi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pglmrsub.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2snsxesvm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wnqyioag.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bnluetqx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lmkjgyuo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ypowgkyg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lujwptgf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2opqzswpl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vzqvgzdy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bdcddbve.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2txyfovjc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mzwnjuyg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wmfiuywg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzlugfgl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xlhsqjfy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjawrgl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xvjqnrbr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gqbtrwku.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2mrsubkny.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2yizncbar.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qweptshg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2olvosaza.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ypqmscfs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2enxeoqfe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wlyhnvyp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bzrnvpzk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tieljljp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hsypfwsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jghobseq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2atfjavxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgilrcji.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jqsiclvm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dofjvyfz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ljnwflfu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nqpcdyed.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vbuetovl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ppysuzzu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rypcjdhu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mociuifk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nrxowzko.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2njofleoh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ksqcxwxw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ljldmjyl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2elgdopkm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mnnaqtas.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qjdswarp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rsgeiiur.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mnmlaybj.html


<!-- 参考信息 -->