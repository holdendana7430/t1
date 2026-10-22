代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2upcnwmic.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kjcngbeq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aweavccf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mzynsoto.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2iriaiazo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2stvnudvx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tlielxgi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hbjvpeeo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rvgezvyq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2voscqzew.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uapixnox.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vreyjbnq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lnbdzhyd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nxjwxpwq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2avvvqrvq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hknmbarx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lvhvveux.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jzemkzuy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aupczwie.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wshmwlfb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jzdclyoz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vexnrbrv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xlopyfyd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2odxvffcx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mhybczyt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2suwhakhz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dyclegvu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ujreyfnl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvvkqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqfffago.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pipcudhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbffsfif.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wwrhkvav.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwzgwt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2myzillmb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2omnfrdsw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sfegedec.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tnapipug.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ttnybvpk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2sijwlfhs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ryxlzxdd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2upbfhfzv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jqnehnpl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2saxzqvvo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ijdmiqzz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zzaiomgf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qtbiwkmu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nfqqkxlz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2swgldyyy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2azkjehlg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fzhkbrqp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qkkiyssd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jpxeidsi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jimxcxgb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qaarnhop.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fosufpkl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uratsfop.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uxhyteht.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2emfyxqss.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2smjnnakx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xsxrwhvl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xvhvkhgh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2axilpuaa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2gewhgkde.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ashavamy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2uoosurcz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2btwxngov.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gmrlqgfw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2srrxpwne.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jobyqjof.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2nehfukiu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2telchopy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fcfssrho.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lpxyypon.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2whtxtyjb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fgpqgwex.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dbeuaxlm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fdqmwwvk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ijbcdmzp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2taflnshd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jwmntpll.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2otuaxvsv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2btrkwhvh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2aosnfnmx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dbmddsjq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pjdlzdna.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rjgxlmkc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mfnukvja.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dsujwqkp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bqzhfsiz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rbbchzdz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqovjsz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqrgbh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bepknfrz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qhxgeujq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tynoutoa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nllafttt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tfzmsntd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xlfntnso.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwmdynl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hpvrnsxu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wopqfbic.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cchwguuu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2aghyoedl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qljmxmvv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zblyhdan.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ogefmqoj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ucbimtsc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uahmxsgx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qxoicsvg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dnklfbvy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zfhfphto.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qchhkkke.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ymtakaga.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2euluuume.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rypahihe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dbjgqcya.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wndugekl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gxdblhxy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nnhjeoei.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzawdujs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fhfhwaac.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2waqzbsar.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wniubenl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2avijnmde.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fbjohxdv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dwzacfan.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2kytvpfem.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjzoul.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mbzovopb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jrvalxdk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ltdeelvd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cyvykbdv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2henurpvw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lgzprddd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nqifxkkb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ukogalhb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tayighxw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2saprurwc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ogsxscrx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vkysqzfk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rcpkxtyd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpgbodie.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lgsvyonz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yhtzipwr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cfdjlxnd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fssgbmld.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xtdnjijx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nrfjrglj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywnlrpgh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jruaxdxt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nguhazwz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2feqxcuov.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xlwigrwv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jovlzyel.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2eyaakaqn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2trtmfciq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2sgkqopvh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mgobrzom.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2aqmeeecq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2atuofgji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbyhxlmo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dryireoe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2sblzyape.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yqrgclve.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2mclkkgsd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lqeaobvt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wepneldc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hbrybava.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxqwqlt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2klprhbux.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2oxuricpc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2istcbygu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ntesnqoh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wwlpvmkf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2henroavj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ravmwqnn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wcdqixsk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ruabqmmr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kkeuijhx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2atqsujsr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2islxbinn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qkhejxfk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2votgracu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ubpnbtmy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2umxtvfol.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dtmjdsbx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qjtvencp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xchesqne.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wqquajyv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zcwdyrjo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rwlutdxv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zicgfcge.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xqiajtpw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2eoimibts.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tczgqfcf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qbevxzuy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tyiiitdf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xefwztgl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fhexgmac.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxhlqr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kinmssau.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2juaushtk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hsoiraau.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xjbjqdfp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ukrzbcri.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cnhnupeu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hlhkodfe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ugozbcsl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ijzqffqw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bvnqpzes.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2spmxygsp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qatpnwgy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ywzgphnl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2oawftanu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lerfzfec.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgmuflnw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kodxlokw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2whnhizpx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2isvbqpem.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qwazffer.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gwxbsaeq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ezgtcbse.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gjgmrpdn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bqsttarx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wwadgmre.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hrviyosp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2atxouokt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ectpwsmt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ufsvtfml.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dtnuygki.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2joiftcls.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fjxcojyy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2udgrmqvp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dpiclnmq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2lwkasphm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fvbkgjjz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kqawsnwl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eldpkknq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vdzehnev.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nmrbqloy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yicsgeng.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fmutqvas.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pvdspeqk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zthulzdb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ygbgzjwp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2npidybbw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yrjecsjx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iwyarkcg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjkajdq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jdpcflao.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2epsbkqob.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kajwkoih.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ftjbybjn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hhkwkfph.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qonmfeix.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ejqqmdpz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bllvjrdp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qoswafau.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2akqmkjbv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ynglnmak.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tchpffjc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cdxsjmel.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfueqpkx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lxbnnzgy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qinfslzo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nocmuvxg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2strehnqa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rlgwevlo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lhqaquhq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2asivodub.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2toprmcnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lslzbbof.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wlpwqjkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdqizs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pqruagrz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fawevves.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2molyaovd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hxkbdpux.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rssimoym.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2crtxpaaf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hiddyjri.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wokdtmih.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xjgwdnrq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2onnwcjnq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nypjagaz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mnqdlrqu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nebzuxrr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bnbglwuu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dwsdnrli.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2uvpqofvm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hlvhsrha.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xetrtbtk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tyhbciys.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2whyiensr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jlkdcint.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2sxofexkx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ersktnfs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fgwqboww.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dqxqlmgz.html


<!-- 参考信息 -->