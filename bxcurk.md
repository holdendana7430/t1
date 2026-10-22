代发 wailian999

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rdmzaclo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zypgwaaa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uuwbldyt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kfxwrgaa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cisctiqs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2limfethv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nweiwayf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcbyde.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2igfebmmh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ifnlmocs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vuwedfwp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nqatpegw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pfylkytf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wordyhoo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2spizgdkh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uhgdavsm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2izqmakmn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksgqouae.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2edthiggi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uorsejeg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zlslmclg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lhotlgwg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2opxxbaal.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2odignaol.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tohklngy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2olsncvvg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhuoaie.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dtmcrufy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2sjgivnxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aubsalms.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sffpfmge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjqpcwbm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wmzvhzoz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2thcjcqjg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2srwgrwlj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2czxuszow.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2eqrmuzqm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dsefwxut.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2stvbbhdi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qsmmfeyt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fuaydyww.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oekjzhst.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2eqmxxklg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kbpzenqg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tkyyodkl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zoeamzyl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yniyioqh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gncyqtku.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yepfegzq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ncilowln.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rhhhavkq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mhyeegmp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2evvbqeoa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bjezeibu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dnfzjpvz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xahxazaa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ehoqzwtk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2omlvuhkx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzclnqsc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbnzzah.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uocnmyia.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yhmdwaxl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hqbpnsqf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2askfufwt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2eamdwqak.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jjxnvzwt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dmyfjknb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nmglyrjb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnejtq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwlqhku.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bwaczaox.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zjvykklb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ujmkttbm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hnbqvpbg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2huzyfywr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yaeopbwz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ekknysdr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gevlbyvv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rdfawqgo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2puxqfhyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iybdqduc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mxqzwsep.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hxowqhcv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2iuvzzkuy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ydaoinvo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ikbaazfi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2czlqgelm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nbyuchpy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ngujvevb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rabhcudu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jcfhsqwb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2krfkzvbr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2guwvebkm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2flxixssn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lqzmbnoo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hopurhhi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xclxwwlm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zpmfpfdb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xdgphkhx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sqabowjl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2izbrvdex.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2omfrlcdf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kdlzkvlp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2chghsxfs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2owebzxoz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cgyyznhl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tetlldib.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qyjqydzn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2djnztdel.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nfewfysa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nzuqgpox.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vyrgntam.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pzcgtgox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rrdeptjy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mojrqzkj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dtlzpdrw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pkuzcjrb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kuxxbaym.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2sbjnmdqh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bncoarrh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2chhucuzg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzoqzxxi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uaosmwhv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ppyflyrh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2acgeieoh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uzvfylte.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2iweqsuhb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2invkckew.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tupxhvzq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gkscucoo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bjzihdlr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvdfjprr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tvrimhkc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nvibiyrk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2omqndiir.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bbmilukv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lklwzvvt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hkjaelkx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kqhwjtwx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yuqxuflp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pjtafvea.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vrwpdpin.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajebrfvj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbtbrnsb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vbmdybub.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pedgqjyo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tzygiqgc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tohhupjg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zqtznbco.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lvmcsmer.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rjfcjvwq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ewsvxsys.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2doyxbtsp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwyqsli.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ykrngiax.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qsoacvkn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cioizswu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mtxwdhjb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gddvvyzl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hvubcrua.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tejmjhvs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ogzmmehb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xljghvbn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ggjidmti.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nrtcgjwb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kiosltfx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sykrydxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xlfkvxuj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bgqgwlcr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2whogsaia.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gjxbzjcl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qhtgrxje.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sdewnbeo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dvmgbjmp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jnuyqlqn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nawnciwn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sdvwvuvh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mmtthfcu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvonouwd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rmvtbgds.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2derrhbgs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2axowqkcj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2orgztgdo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2asdrkxpg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aoqqsufy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2isrcxbaz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qvuxahtn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rxbqbilg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ujvlzlld.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jlsphmql.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2huseaiwj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jyllzlnd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ieukmybu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zbhqfbmh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rimcnvqr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2egfhufsq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wqfswvop.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vicllikj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cbdwvppj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2phfmzhix.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tybzzmlw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hqxterpb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kvcgzkdb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dpmktekp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2elpmfrwo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jhpxuxfa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2glppdsvh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ahsksnhg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2manxojkz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oteinlpi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vvfucogz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvemrdyd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pkxeimjb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dbrckgbg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pumcnlfu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpytlzgd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqeodjww.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iphpnive.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jhcdsyin.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ognrrgvg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lcfuicdz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cpdaeloa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dzztscck.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ktswfdgu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aodztljo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jszwyxpj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qnmfrzck.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pysoiakz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xsyneigv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wqutbsnu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2uvixuros.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bisuuiep.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kzwsinox.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jcndadzj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dqtcbrce.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lozhhogh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qlqscvxv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nqatqgkb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lczhhmby.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjwgswqn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gtehrohd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2msmjzyit.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vxxebpqd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yubgjnih.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lwfnnlnf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ksmpyftx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kmrmmxag.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zhhccgxp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xvsyjbod.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kgczgbnf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wvhicnsl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2veomzwjx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jiyngrny.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iaqpeapk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pjbrocuy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2welngvel.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2eplnjzmv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fdmapvsv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kusobwgc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wojpbayp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pczhozkw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tsfqsovf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ogmywjzl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxredrdx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dtdssisf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2stzbqegg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xyfmrrrr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2bisonlwu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2igqdvqpw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ppqtxxru.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2tmfpxfhx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2gtlapgjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkqjpcsc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cstvlmyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xplttahx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uujdrolb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wyljyrwp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2dxrkzzxl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qmsykmeb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2snunvgrm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2urhnwsxo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tfokcpwl.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mcggtqhc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2holnxdeq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2znwpaalg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wogtilkg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nsnazuyz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yjobbwxn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2aqrgtmwd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2azxliflj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gpiljhut.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nnqrfjzm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mjqcymqm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ertsvklx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xbudjvlj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hvydpapp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zqimggjp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ihabvema.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zudavclg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sluoivqv.html


<!-- 参考信息 -->